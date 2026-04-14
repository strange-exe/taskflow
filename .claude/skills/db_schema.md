<skill_context>
Database Schema and ORM Standards
</skill_context>
<rules>
- Always enforce referential integrity using explicit Foreign Keys.
- Provide compound indexes for fields queried frequently together (e.g. `user_id` and `status`).
- Use UUID/CUIDs for primary exposed keys to prevent enumeration attacks, or at least BigInt auto-incrementing if internal.
- Define explicit exact cascade behaviors (`ON DELETE CASCADE` etc) where applicable.
- All models must include `created_at` and `updated_at` defaulting to `now()`.
</rules>