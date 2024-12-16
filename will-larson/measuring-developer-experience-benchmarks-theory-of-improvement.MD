
[Link to article][https://lethain.com/measuring-developer-experience-benchmarks-theory-of-improvement/]

#Challenges in developer productivity tools

* Use of productivity to evaluate rather than learn. 
* Integration across multiple tools.
* Forcing a standard model on a unique problem.

## Notes: 

* Measurement of productivity must come from an intent to diagnose and learn rather than evaluate a team or an individual. Measurement for evaluation must focus on other metrics such as value generated vs cost of the team, risks in the organization, team talent distribution, etc.
* Any productivity measurement tool must collect data from multiple sources because teams use multiple tools for their work - ticket management system, code respository, IDE, CI/CD pipeline, etc.
* Measurement tools come with their own measurement philosophy. This philosophy enforces a standard model like DORA or SPACE on an engineering problem that is often unique. The tool must measure and diagnose the problem that I want to solve rather than guiding me to a generic solution before identifying the problem.

There is a correlation between this and the observability problem of distributed software applications. Building a standard logs, metrics, and dashboards O11y system will not solve issues in an application. 

# Requirements for a modern productivity measurement tool

* Inbound and outbound integrations across industry standard tools.
* Graph the metrics in a consistent manner (i.e.,) build a consistent narrative with simple metrics.
* Provide comparison against industry and internal benchmarks to judge the team's performance.
* Provide a “theory of improvement” such that you can roughly translate your scores into the projects to invest in.

### Notes:

* Judgement _could be_ different from evaluation. Clarify this with Will via Email.
* Benchmark driven measurement will lead to a consolidation of tools because only a few tools can become preferred vendors of a large volume of companies to collect the required benchmark data.

# Progress in tools from 2020 to 2024

Will provides a series of Wardley maps showing the progress of the tools and his understanding of the progress. The key takeaways are,

**User classes**

* Engineer - useful insights, minimum effort to maintain the data
* Executive - Judgeable reports that can drive decisions and reporting to board
* Dev productivity team - provide services and make decisions on where to invest

The progress section reiterates what Will spoke about earlier - tools that provide comparisons against benchmarks are the most valuable tools. Takeaway from this - when you try to measure developer productivity, always compare against a benchmark. E.g., how fast is my team releasing to production or resolving defects compared to companies of my size in my domain.

# Theory of improvement

## Judge-ablity vs goal-ability

A judge-able metric is a lagging metric that helps you in diagnosing. Judgement is always against a benchmark of peers. Never judge in isolation. E.g., average merges per engineer
A goal-able metric is a leading metric that you can improve resulting in a change in the judge-able or lagging metric. E.g., addressable tech debt in a particular area of the product which will increase average merges per engineer.

Question: Are judge-able and lagging metrics, and goal-able and leading metrics synonyms? Clarify.

## A critique of [DX Core 4 metrics][https://getdx.com/research/measuring-developer-productivity-with-the-dx-core-4/]

* DX Core 4 provides good judge-able/output metrics. The onus is on the teams using this framework to evolve strategies using these metrics.
* % of time spent on new capabilities is highly useful but difficult to measure. Why?
* Time to nth PR is a highly useful onboarding metric.
* R&D (spend ?) as a % of revenue is a good self evlauation metric for the executive and the board.
* A composite DX metric ([DXI][https://getdx.com/research/the-one-number-you-need-to-increase-roi-per-engineer/], a custom metric derived from 14 different metricsdefined by the DX team) is a useful but expensive metric. Useful because it considers various factors and is derived using DX's research. Expensive because it is difficult to explain.

## Predictions for 2025

1. Reduction or convergence of frameworks. DORA, Space, DX Core could converge. No more new frameworks.
2. Theory of improvement moving from custom to product section of the Wardley map (i.e.,) this value creation becomes more mature.
3. Developer productivity teams move from analysis to doer teams.

# Questions

1. Why does Will emphasize on judgeability after mentioning evaluation as an undesirable goal in the introduction? My hypothesis is that judge-ability helps in diagnosis while evaluation focusses on a preference (i.e.,) In judging metrics I try to evaluate the underlying problem whereas in evaluation, I try to rank and attach value to the metrics themselves. 
2. Are judge-able and lagging metrics, and goal-able and leading metrics synonyms? Can these terms be used interchangeably?
3. Why is measuring % of time spent on new capabilities difficult? Won't it be as easy as separating new features, defects, and maintenance work using some categorisation technique like a label?

# My takeaways

* Use Will's criteria when evaluating a developer productivity tool or even starting a developer productivity initiative in the future.
* New topics to explore - [Wardley mapping][https://lethain.com/learning-wardley-mapping/], [Strategy testing][https://lethain.com/testing-strategy-iterative-refinement/], [DX Core 4][https://getdx.com/news/introducing-the-dx-core-4/], and [Accelerate][https://www.amazon.in/Accelerate-Software-Performing-Technology-Organizations/dp/1942788339]
* Immediate action - drive the QA platform team headed by Kande to do rather than just analyse.
