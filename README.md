# CalgaryPLuse
CalgaryPulse is a living AI simulation of Calgary's entire economy. Citizens click on any building to see their taxes, explore policy trade-offs through an AI sandbox, discover uses for vacant downtown spaces, and vote on city priorities  all powered by agent-based modeling, reinforcement learning, and large language models

THIS IS OUR Agent-based model, RL, LLM, forecasting

Pillar 1 — Living 3D Calgary: Full Three.js scene with 15 real downtown Calgary buildings (Brookfield Place, The Bow, Bankers Hall, Telus Sky, etc.) rendered as a 3D cityscape. Buildings are color-coded by vacancy , red/orange = crisis, green = healthy. Particle effects represent tax flow. Drag to orbit, scroll to zoom, click to select.

Pillar 2 — Building Data (Open Data Ready): Each building carries the exact data structure you'll pull from Calgary Open Data: assessed values, tax rates, vacancy rates, sqft, rent PSF, floors, year built, zone codes, ownership. The panel shows all of it when you click a building.

Pillar 3 — Agent-Based Simulation: Every building is a BuildingAgent class that independently calculates its tax burden, the tax shift it causes to residential homeowners, lost revenue, and an economic health score. The agent factors in vacancy penalty, building age, and the 62% residential tax shift ratio.

Pillar 4 — Fill the City: Hit the "✦ Fill the City" button and the whole experience transforms. Vacant buildings pulse red. Click any one to fill 20% of its vacancy — the panel shows revenue recovered, tax shift reduced, and builds toward the login → request space → owner approves → rent flows pipeline. The CTA at the bottom maps out that exact user journey.
Next steps we should tackle: connecting to Calgary's actual Open Data API for real assessed values, building out the auth/booking flow for the "Fill the City" pipeline, and refining the 3D building positions to match real downtown GPS coordinates.
