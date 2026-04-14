<skill_context>
Backend API Development Standards
</skill_context>
<rules>
- Use Zod or Joi for request payload validation mapped dynamically to TypeScript DTOs.
- Always implement a centralized error handling middleware. Never leak stack traces to the client.
- Return standard JSON envelopes: `{ "success": boolean, "data": null | object, "error": null | object }`.
- Status codes MUST be semantic (200, 201, 400, 401, 403, 404, 500).
- Wrap routes in `try/catch` or use `express-async-handler` to prevent unhandled promise rejections crashing the Node process.
</rules>