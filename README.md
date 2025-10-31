

# 2025_10_31_gdp_capsule_collision_for_fast_projectile

> In a bullet hell game with long-range and extremely fast projectiles, you can’t rely on a single thread or the built-in collision system to handle the massive number of projectiles efficiently.

In Unity3D, I experimented with creating a custom collision system for projectiles:

* Raycasts were too heavy.
* The built-in collision system couldn’t handle the sheer number of collisions.
* A single thread wasn’t sufficient.

To handle this properly, you need to build your own collision system using math-based capsule checks and multi-threading, either on the CPU and/or GPU.

I don’t have the solution yet, but I plan to develop and refine it here in Godot for my servers.

A bit of imagery for inspiration ;)  
- https://github.com/EloiStree/HelloUnityKeywordForJunior/issues/170
- https://github.com/EloiStree/HelloBulletsHell/issues/2
- https://github.com/EloiStree/HelloBulletsHell/issues/4
