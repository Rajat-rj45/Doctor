# MarizFirst Technical Architecture Decisions

## Frontend

- Next.js App Router
- TypeScript
- Tailwind CSS
- Server-rendered public SEO pages
- Client components only for interactive areas

## Backend

- Next.js route handlers
- Service layer for business logic
- Repository layer for database queries
- Zod validation on server
- Prisma ORM
- PostgreSQL database

## Forms

- React Hook Form
- Zod validation
- Visible labels
- Accessible error messages
- Consent checkbox required

## Auth

- Auth.js / NextAuth
- Secure HTTP-only cookies
- Role-based dashboard access

## Media

- Cloudinary or S3-compatible storage
- Store only URL, public ID, metadata in PostgreSQL
- Never store image/video binary in database

## Security

- RBAC on every dashboard route
- Ownership checks for partner data
- Rate limiting on booking/search/auth
- CAPTCHA/Turnstile hook for spam protection
- Audit logs for sensitive actions
- No patient data exposed publicly

## SEO

- Server-rendered public pages
- Dynamic metadata
- JSON-LD schema
- Sitemap
- Robots
- Canonical URLs
- Internal linking

## Deployment

- GitHub
- Vercel
- Managed PostgreSQL
- Cloudinary/S3
- Sentry
- GA4

TRD recommends modular Next.js architecture with services, repositories, RBAC, secure patient handling, public SEO pages, PostgreSQL, Prisma, official WhatsApp API, Cloudinary/S3, Vercel, and monitoring.
