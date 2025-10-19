# Service Flow

```
USER REQUEST JOURNEY:
┌────────┐    ┌─────────────┐    ┌─────────────┐    ┌─────────────┐
│  User  │───▶│ Next.js     │───▶│ NestJS      │───▶│ OpenAI      │
│ Input  │    │ Frontend    │    │ Controller  │    │ Service     │
└────────┘    └─────────────┘    └─────────────┘    └─────────────┘
                                                   │
              ┌─────────────┐    ┌─────────────┐    │
              │ Response    │◀───│ Formatted   │◀───┤
              │ Display     │    │ Result      │    │
              └─────────────┘    └─────────────┘    │
                                                   │ Fallback
                                      ┌─────────────┐
                                      │ Database    │
                                      │ Service     │◀──┐
                                      └─────────────┘   │
                                              │         │
                                      ┌─────────────┐   │
                                      │ SQLite      │───┘
                                      │ via Prisma  │
                                      └─────────────┘
```
