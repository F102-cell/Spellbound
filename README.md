# Spellbound: King's Realm

Play the game here:

https://f102-cell.github.io/Spellbound/game.html?v=1.01&build=enemy-guide

The Enemy Guide on the main menu shows each enemy's appearance and attack style.

Online matchmaking, ready-up, private parties, and synchronized PvP require the
Supabase schema in [`supabase-schema.sql`](./supabase-schema.sql) to be applied
to the project. Public matches and invited parties support team PvP (1v1, 2v2,
3v3, and 4v4), free-for-all (2-8 players), and co-op survival (2-4 players).
PvP players complete an Easy survival stage before combat; teams are randomized
for team matches, while every free-for-all player is an opponent. Co-op players
share enemy waves at a selected difficulty from Easy through Impossible.
Friendly fire is off by default and can be enabled for team PvP or co-op.
Variable-size lobbies start when the host starts a ready lobby with at least two
players. Leaving a live match for the main menu applies a 10-minute multiplayer
penalty. Multiplayer leaderboards track total wins separately for each mode.

Community posts and live chat also require a signed-in account and the schema's
community table permissions. Leaderboard updates use Supabase Realtime.
