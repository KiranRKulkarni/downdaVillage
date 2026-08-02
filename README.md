# Down da village booking admin

## Start locally

1. Copy `.env.example` to `.env.local` and add the Supabase project URL and publishable key.
2. In the Supabase SQL Editor, run `supabase/schema.sql`.
3. Run `npm install`, then `npm run dev`.

Down da village is configured as one 40-unit inventory in `src/data.js`.

| Category | Units | Room numbers | Floor / location |
|---|---:|---|---|
| Deluxe Room | 3 | 01, 02, 03 | Ground floor |
| 2BHK Villa | 1 villa | Villa | Ground floor |
| Standard Room | 14 | B1–B7, C1–C7 | First and second floors |
| Family Room | 6 | B8, B9, 101, 102, 103, 104 | First floor |
| Family Quad Room | 6 | C8, C9, 201, 202, 203, 204 | Second floor |
| Deluxe Quad Room | 10 | 301, 302, MH1–MH8 | Third floor |
| *Total* | *40* |  |  |

The included RLS policy is deliberately for a quick prototype; enable Supabase Auth and replace it before deploying publicly.
