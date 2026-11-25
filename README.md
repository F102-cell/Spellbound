# Spellbound: King's Realm

Play the game here:

https://f102-cell.github.io/Spellbound/game.html?v=1.01

Online matchmaking, ready-up, private parties, and synchronized PvP require the
Supabase schema in [`supabase-schema.sql`](./supabase-schema.sql) to be applied
to the project. Public matches and invited parties support 1v1, 2v2, 3v3, and
4v4. Every player must finish the Easy survival stage before the shared team
combat begins; teams are assigned randomly when a match starts. Friendly fire is
off unless the match creator enables it. Leaving a live match for the main menu
applies a 10-minute multiplayer penalty. Multiplayer leaderboards track total
wins separately for each team size.

Community posts and live chat also require a signed-in account and the schema's
community table permissions. Leaderboard updates use Supabase Realtime.
