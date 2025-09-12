# Stage 1 — Build
FROM node:20-alpine AS builder

WORKDIR /app

# Install deps first (better cache)
COPY package*.json ./

RUN npm install

# Copy project
COPY . .

# Build Nuxt for production
RUN npm run build

# Stage 2 — Run
FROM node:20-alpine AS runner

WORKDIR /app

ENV NODE_ENV=production

# Copy only built output & node_modules
COPY --from=builder /app/.output ./.output
COPY --from=builder /app/node_modules ./node_modules

# Nuxt 3/4 runs from .output/server/index.mjs
CMD ["node", ".output/server/index.mjs"]
