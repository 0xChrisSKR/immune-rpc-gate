# Lessons Learned

## Reliability needs explicit modes

Systems become harder to trust when they silently degrade. Naming modes such as Normal, Degraded, and OFF makes risk easier to explain to both users and engineers.

## Read-only is a useful safety boundary

When a dependency is unstable, the system may still be able to serve safe read behavior while blocking mutation. Separating read and write paths makes that decision clearer.

## Failure should be visible

Returning a clear unavailable state is better than allowing a user to continue through an unsafe or inconsistent flow.

## Infrastructure design is product design

RPC health, state consistency, and failover behavior affect the user's confidence directly. These concerns should not be treated as invisible backend details.
