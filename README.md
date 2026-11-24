# Spellbound: King's Realm

Play the game here:

https://f102-cell.github.io/Spellbound/game.html?v=1.0

Online matchmaking, ready-up, and party invites require the Supabase schema in
[`supabase-schema.sql`](./supabase-schema.sql) to be applied to the project.
Public matchmaking is open to players in the selected mode; private matches are
created as parties and can only be joined through an accepted party invitation.
The host can start either type of match only after at least two players have
joined and every player is ready. Community posts and live chat also require a
signed-in account and the schema's community table permissions. Leaderboard
updates across players use Supabase Realtime and require the schema to publish
the leaderboard table.
