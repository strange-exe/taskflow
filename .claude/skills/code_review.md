<skill_context>
Code Review and Quality Assurance
</skill_context>
<rules>
- Review must fail if any `console.log` exists in production execution paths.
- Ensure 0% usage of `any` types in TypeScript.
- Verify that every endpoint defined in `architecture.json` exists in code and matches the schema exactly.
- Verify environment variables are loaded securely without hardcoded secrets.
</rules>