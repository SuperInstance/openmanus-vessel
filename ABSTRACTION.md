primary_plane: 4
reads_from: [4, 5]
writes_to: [4]
floor: 4
ceiling: 5
compilers:
  - name: deepseek-chat
    from: 4
    to: 2
    locks: 7
reasoning: |
  Openmanus-vessel is the web scouting agent operating at Plane 4 (domain language).
  It navigates and explores web resources using Domain Language notation (4) like
  `NAVIGATE[url] SCRAPE[selector]` commands, and can receive high-level Intent (5)
  instructions. Outputs remain in Domain Language for fleet coordination.

  Floor at 4 means openmanus-vessel works exclusively with structured domain
  notation, not lower-level IR or bytecode. The Domain Language layer is the
  sweet spot: high enough for human-like commands but structured enough for
  fleet coordination. The compiler to Bytecode (2) allows converting scouting
  patterns into executable skills for autonomous web missions.
