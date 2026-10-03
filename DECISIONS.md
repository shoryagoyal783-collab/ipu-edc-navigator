# DECISIONS.md

## Design decision: Dijkstra instead of BFS
I chose Dijkstra because walking connections can have different estimated costs. BFS is appropriate when every edge has equal cost; Dijkstra handles non-negative weighted edges and minimizes total route cost.

## Edge case: unreachable destination
If no path connects the selected start and destination, the app reports that no route was found rather than displaying a partial route.

## Map accuracy
The map is illustrative and not an official surveyed map. Exact positions and paths—including Chill Zone, EDC Chowk and individual rooms—need verification using campus signage or an official detailed map. Costs are relative units, not metres or real walking time.
