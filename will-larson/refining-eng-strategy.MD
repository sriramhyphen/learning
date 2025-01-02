
[Link to article](https://lethain.com/refining-eng-strategy/)

# Introduction

* Fire bullets, then cannonballs - cheaply test ideas before committing to them.
* Strategy refining techniques - strategy testing, systems modelling, and Wardley mapping

# Why strategy refinement?

* Strategies succeed because they address narrow problems within broader strategies (i.e.,) address the small problems that matter most within the broad context. [Pareto's principle](https://en.wikipedia.org/wiki/Pareto_principle).
* Strategy refinement identifies these narrow problems that matter the most.
* Even if the right problem is identified, the strategy might not hit the right solution. E.g.,
    * Stripe's challenges with planning for work over a month. The problem identified was the lack of a shared planning paradigm. The solution applied was rolling out agile and training managers. The solution only addressed surface issues when a more apt solution would have addressed stakeholder communication and expectation management.
    * Uber's service adoption strategy. Not a lot of detail about the problem and solution in this article. But my assumption is that Uber's infrastructure team was driving adoption of a new platform. This was done by a two part refinement - identify what parts of the adoption were most crucial, and learning by migrating individual teams to the platform instead of migrating en masse. The itneresting takeaway in this case is thatthe lack of authority forced the infrastructure team to refine strategy. Constraints often fuel better decisions.
    * Comparison with Betterworks - Our monolith to migration services strategy also suffered from the challenge of balancing enterprise customer commtiments versus migration and new feature development. Our CPTO addresses this by,
        * Creating a shared vocabulary for our planning
        * Separating true customer commitments from assumed commitments. E.g., A customer demanding feature X hasn't seen the equivalent feature in our legacy system. So, the same feature could be delivered with lesser scope as long as it solves the customer's problem.

# Why is refinement skipped?

Will elucidates my point about constraints here. 

* Teams and leaders with lesser authority have to prove their strategy before implementation. So refinement is mandated by default.
* Executives can mandate adoption of a strategy. 
* But they skip refinement because perception matters more than results.
* Refinement is also skipped because commitment to a strategy is assumed final. Even in my own experience this hasn't been true. E.g., Betterworks' compensation management strategy has been refined multiple times in multiple ways after the initiatl commitment.
* Refinement is also skipped because of lack of proper tools.

## Some asides

* Permissive strategy organizations - organizations where aspirational initiatives and staff projects are welcomed and even required for career growth
* Question to self - how much does India engineering's career path encourage poorly refined staff projects? Past failures - practicing system design, integration platform, etc. How to develop careers without pushing towards a staff project?
    * Some answers
        * Stop owning careers of senior/lead engineers. That's the manager's realm. 
        * Suggest staff level initiatives rather than mandating them. 
        * Mandate only those initiatives which can create immediate business value.
        * Celebrate glue and mentor staff archetypes and not just doer archetypes.

# Strategy refinement toolkit

_Caution: Use the techniques as tools of learning and discovery. Do not become the devotee of any specific tool._

## Strategy testing

_Ideal for ambiguously defined problems_

* Identify the narrowest, deepest available slice of strategy. Iterate until there is evidence of the strategy's success.
    * E.g., smallest possible release for a migration
* Identify metrics that give you evidence of success.
    * E.g., improved customer NPS,  faster response time, or lower MTTR
* Assume people are well-intentioned and it is your strategy that needs fixing.
* Continue refinement until you build conviction or change the strategy.

## Systems modelling

_Ideal for discovering leverage points in a complex system_

* Modelling systems as stocks and flows.
* Need to learn and experiment more on this. This is currently my most preferred and well-understood technique of modelling.
* My knowledge gap - I understand the theory of systems (hierarchical, self-organizing, resilient, etc.,) but not the practicality of modelling them
    * Define a new quarterly OKR for developing Betterworks product knowledge and modelling the product using systems modelling for Q1 FY 26.

## Wardley mapping

_Ideal for understanding how your strategy fits with a changing ecosystem. Useful for problems focussed on adapting dynamic technologies or long-term strategies._

* Understanding this needs more study. TODO: Add a link to Wardle map notes when that is completed.

# Strategy refinement anti-patterns

* Skipping refinement.
* Manufactured consent.
* Optimizing for a side-goal

# My takeaways

* I am a beginner in strategy. Learning and implementing true strategy will be half a decade or a decade's effort. The current hypothesis is that this is something I am interested in, the market would want from me, and I can pursue. I'll refine this hypothesis in the coming years.
* I must practice systems degin rather than sticking to the theory.
* A new hypothesis is that I am doing too much strategy and driving too much change. In 2025, make a commitment towards lesser change, lesser projects for visibility, and more impact. Track what initiatives I own. Own only initiatives that truly matter to the business.





    



