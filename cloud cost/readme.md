
Original PDFs with images can be found here:

[English](https://github.com/canada-ca/TBS-OCIO-ESP/blob/master/cloud%20cost/GC%20Cloud%20Cost%20Management%20Playbook%20Published%20July%202022.pdf)
[francais](https://github.com/canada-ca/TBS-OCIO-ESP/blob/master/cloud%20cost/Guide%20sur%20la%20gestion%20des%20cou%CC%82ts%20de%20l%E2%80%99informa%20tique%20en%20nuage%20du%20gc%20publie%20julliet%202022.pdf)

[(francais)](#francais)

GC Cloud Cost Management Playbook
=================================

# Purpose

The purpose of this document is to:

-   Support Government of Canada organizations adoption of cloud while applying financial due diligence while maintaining agility

-   Provide a set of practices to maintain cost management in the cloud without negatively impacting agility and other cloud attributes

-   Providing stakeholders with an overview of cloud cost management including financial & procurement officers

# Context

Cloud computing provides on-demand, pay-as-you-go models for computing, storage, network, platforms, and business solutions. Cloud costs are fluid and directly related to the unit price of the resources multiplied by usage (cost = price x usage). This represents a fundamental shift from traditional, fixed, IT consumption models where the primary cost is associated with the purchase of hardware or licensing of software. In a cloud model, cost is a direct input into application architecture. Cloud spending is much more dynamic than traditional IT models as usage changes result in immediate cost changes. The feedback loop between usage and cost is immediate. Traditional spend controls rely heavily on process gates with people-intensive oversight. These traditional practices are a poor fit for a cloud environment as they can negatively impact the agility delivery teams desire when using cloud and lead to disrupted business value. Finance and procurement officers are not gatekeepers to cloud spend, but support delivery teams in establishing budgets for the delivery of their products. Delivery teams are directly responsible for cloud costs and must be prepared to track, analyze, and optimize the costs associated with their products and the usage of those products. These practices are often known as 'FinOps'. FinOps is a set of practices that encourage management & optimization of cloud spending without disrupting the agility and speed of cloud delivery.

# FinOps

Often the term 'FinOps' is applied to cloud cost management. FinOps is a portmanteau of Financial Operations. FinOps is supported by a community lead [FinOps Foundation]. The foundation and technology consultancies have published a library of information on this topic. This guidance should not be read in isolation of that library of material. FinOps is an evolving area as cloud itself evolves.

# Traditional Models Contrasted with Cloud

One can thinking about the shifting from traditional IT models to a cloud model using the analogy of shifting from digging and maintaining your own well vs connecting to the municipal water supply. Both deliver water, but each has a different model behind it. With a well, you must take on the responsibility of purchasing equipment, engineering, and building the well, and be responsible for maintaining the pumps and quality of the water. With a municipal water supply, you simply pay a monthly metered water consumption charge, and you are abstracted from the assets required to deliver the water. This, in many ways, is the shift that cloud has introduced. Traditional IT models, like digging wells, is a capital and asset intense delivery model. Cloud, like municipal water supply, turns the supply into a commoditized service.

The table below assumes that the pay-as-you-go (PAYG) model for cloud has been maintained. It should be noted that depending upon how your organization structures its agreement with providers, portions of this table may not apply. For example, if through a contract the consumer pays for years of services up-front, portions of this table will not apply. Furthermore, this table's scope are the cloud services themselves, and does not include capital costs for implementing the services or extending/building within these platforms.



 | Traditional IT Models  |  Cloud Models |
 |------------------------|---------------|
 |Traditional IT relies on a Capital Expense model (CapEX) where goods (software, hardware, facilities) are bought, maintained as an asset for a determined life span.|Cloud service are an Operational Expense, much like a utility such as electricity or municipal water, the degree of usage drives cost.|
|The degree to which an asset (hardware and software) is consumed has no material impact on cost. Once a purchase is made, the costs are sunk into the asset and there are no mechanisms to optimize those costs after purchase.|Consuming cloud resources results in costs. Turning off the usage of a service results in cost avoidance.|
|Traditional investments are typically periodic associated with the replacement of aging assets. |Cloud costs are in perpetuity until the service is turned off.|
|Traditional models are primarily fixed costs.|Cloud costs are variable.|
|Traditional costs reporting is periodic, often annual as costs are largely fixed.||Cloud costs are real-time as they are variable|
|Traditional models have straight forward cost driver. |Cloud bills are complex often comprised of micro-transactions tracking each usage.|
|Purchasing of capital assets are centrally gated by procurement and financial organizations.| Cloud purchases are decentralized being made by delivery teams delivering digital products with the cloud.|

  
  

# Optimizing Cloud Costs

When contrasted against traditional IT models, cloud allows for more options for shaping spend. Levers in the form of optimization decisions can be taken to reduce waste and right-size consumption. Conversely, decisions can be made to spend more to get greater speed and scaling. Optimization choices can be plotted on a simple quadrant to illustrate the trade offs between time and cost as seen in figure 2. Optimization is focused on reducing waste and shaping spend. Continuous optimization may not lead to reductions in overall cloud spent over the long-term. Often, organizations continue to grow their cloud usage with time in the form of new services, new data, and new user experiences. The increased digitization of an organization's business will, over time, result in an overall increase in cloud spend. Optimization can help ensure that spend is well governed and not resulting in needless waste.

## Feedback Loops

A key attribute of how costs are managed in the cloud depends upon the real-time feedback loop between using cloud and cloud costs. This simple feedback look drives financial behaviours that can lead to optimizing cloud usage to reduce needless spending.

## Business Value, Not Lowest Cost

The goal of cost management is not to drive to the lowest cost but instead:

1.  Optimize unnecessary waste

2.  Delivery business value

Driving to the lowest cost possible can impact business value. Delivery teams and business owners may be willing to trade higher costs for quicker delivery. For example, a delivery team may decide to deploy an architecture that is not optimized because a simpler architecture may lead to faster delivery of a solution. The trade-offs between potential savings and the effort required to achieve those savings is illustrated below. Another example is prioritizing the launch of a new feature may be deemed higher that refactoring a piece of code that could lead to lower cloud costs. Therefore, opportunities for cost optimization become part of a product's feature backlog like. Opportunities to optimize a product for cost must be prioritized with other backlog items like new user experiences, new business rules, and other feature requests.

Managing cloud costs is not about driving to the lowest cost, but instead applying financial due diligence while driving business value for the organization.

# Plays

This document contains plays that organizations should undertake to exercise due diligence over cloud spend. This is not a comprehensive set of practices, but instead represent suggested, minimum practices.

|No.          |Play|
|-------------|----|
|01           |Accountability|
|02           |Visibility & Transparency|
|03           |Cost attribution|
|04           |Budgeting|
|05           |Service Policies & Alerting|
|06           |Optimization|
|07           |Cost remediation|
|08           |Governance|
|09           |Set business metrics|


# 01 Accountability



## Objective

Delivery teams[^1] must be ready to assume cost management and optimization responsibilities. The implications of architectural designs and provisioning choices need to be understood by delivery team members.

## Description of Activities

-   Ensure delivery teams are aware of the impact of their consumption, configuration, and architectural choices have on costs

-   Consider setting a cloud financial management (FinOps) training requirement for all delivery team members

-   Ensure the basic concepts of FinOps practices and the guardrails listen in this document need to be understood by delivery team members

-   Use the GC FinOps RACI (link required) as a template to tailor to your organization's roles

-   Determine a centralized role within your organization who will manage cloud spend data and decisions with your organization's governance. This does not need to be a dedicated role, but part of a Cloud Centre of Expertise's responsibilities.

-   Determine the role of financial officers in your organization's FinOps practices

## References

-   <https://finops.world/en/organization-and-key-roles/>

-   <https://finops.world/en/practices/card/1s1-assign-the-2-first-roles/>



# 02 Visibility & Transparency


## Objective

Empower delivery teams with self-service access to cost reports. Delivery teams must have complete visibility into the services and usage that is driving cloud service costs associated with the delivery of their products. Be transparent with all stakeholders on cloud costs.

## Description of Activities

-   Provide reports and dashboards on past, current, and forecasted cloud spend to stakeholders

-   Provide a standardized cost reports to all delivery teams, but allow delivery teams to tailor those reports to their needs

-   Provide reports in such a way that a delivery team can isolate costs associated with the delivery of their products

-   Maintain visibility over all cloud accounts and cloud services. If your organization uses multiple cloud providers, visibility over all providers and accounts will need to be maintained.

-   Provide all stakeholders with transparency on cloud costs

-   Determine how high in the organization cloud spend data should reach. For example, does the CIO or CFO have an interest in monthly reports?

## References

-   Cloud FinOps: Collaborative, Real-Time Cloud Financial Management by J.R. Storment and Mike Fuller

## Automation

-   Check to see that the billing dashboard or API is being invoked on a periodic basis

-   Check that the developer and architect roles also have access to the billing console and APIs

# 03 Cost Attribution


## Objective

Establish a structure for tagging cloud resources and attributing costs back to the lines of business and cost centres funding those costs.

## Description of Activities

-   Document and approve a standardized set of tags to identity how the cost of resources is attributed back to applications and lines of business for billing proposes

-   Document and approved a resource hierarchy structure or groupings that support attribution of costs back to lines of business for billing purposes

-   Use resource tagging and structures to act as reporting dimensions so that costs can be attributed back to lines of businesses and fund centres that fund the delivery of products

-   Search and remediate any untagged resources or resources that exist outside of cost allocation structures

-   Maintain the hygiene of resource:

    -   Identify and remediate orphaned resources

    -   Use automation through the implementation of service policies to enforce tagging hygiene where possible.

-   For common cloud platform resources that cannot be attributed to a single product or line of business:

    -   Determine a methodology for attributing common costs, for example:

        -   Proportional; based upon relative percentage of direct costs (e.g., 10% of direct cloud spend)

        -   Even split; split total amount evenly across products (e.g., common costs/number of products)

        -   Fixed; like even split, but with a co-efficient to weigh the proportion allocated to each product. Total of all coefficients must add up to 1. (e.g., 0.3 of common costs)

    -   Determine a show-back/charge-back methodology for making common costs visible to each product

## References

-   <https://aws.amazon.com/blogs/aws-cloud-financial-management/cost-allocation-basics-that-you-need-to-know/>

-   Cloud FinOps: Collaborative, Real-Time Cloud Financial Management by J.R. Storment and Mike Fuller

## Automation

-   Check for resources that do not have approved cost allocation tags

-   Use service policies to enforce mandatory cost allocation tags

# 04 Budgeting

 

## Objectives

Delivery teams establish product budgets in collaboration with financial officers and undertake activities to track actual costs against forecasts.

## Description of Activities

-   Delivery team will work with financial officers to establish a budget for their product based upon estimated cloud hosting costs

-   Budgets should be broken down by billing period. Alerting should be implemented to notify delivery teams when a pre-determined percentage of the monthly forecasted budget is spent,

-   Delivery teams should report actuals against forecasts to determine if the 'burn rate' is within forecast.

-   Governance should be documented to include process and criteria for increasing budgets.

-   Governance of budget should allow for unplanned usage and costs, but also take corrective action to help delivery teams with repetitive unplanned spend.

## References

-   Cloud FinOps: Collaborative, Real-Time Cloud Financial Management by J.R. Storment and Mike Fuller

-   https://aws.amazon.com/blogs/aws-cloud-financial-management/beginners-guide-to-aws-cost-management/

-   <https://docs.aws.amazon.com/cost-management/latest/userguide/budgets-create.html>

## Automation

-   Check that the cloud service providers' features for setting and alerting on budgets have been configured

# 05 Policy & Alerting



## Objectives

Use alerts to provide early warning when key financial milestones are met, such as percentage spend of total budget. Use service policies to enforce key financial guardrails such as adherence to tagging standards.

## Description

-   Use cloud platforms' ability to alert users of financial events as a method of automating governance activities

-   Use service policies to enforce adherence to key financial guardrails such as tagging and automating turning off services, in particular for test and development environments. Financial guardrails differ from the GC Cloud Guardrails as they are department specific and focused on financial governance.

## References

-   Cloud FinOps: Collaborative, Real-Time Cloud Financial Management by J.R. Storment and Mike Fuller

-   <https://cloud.google.com/billing/docs/how-to/budgets>

-   <https://docs.microsoft.com/en-us/azure/cost-management-billing/costs/cost-mgt-alerts-monitor-usage-spending>

-   <https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/monitor_estimated_charges_with_cloudwatch.html>

## Automation

-   Set alerts for accounts or resource groups based to notify delivery team members when 25%, 50%, and 75% (or whatever values best suit your context) of the team's total budget has been consumed

-   Set alerts for excessive percent changes in costs occurring in a short period of time



# 06 Optimization
 

## Objectives

Delivery teams should continuously analyze opportunities for optimizing service usage and architectures for cost efficiencies. Centralized FinOps teams can discover optimization opportunities to help delivery teams make optimization decisions.

## Description of Activities

-   Delivery teams will review cost and billing reports for possible optimization opportunities and waste

-   Determine the benefit verses cost of implementing optimization strategies

-   Opportunities to optimize architectures and usage should be added to the product's feature backlog to be prioritized along-side user feature requests and technical debt remediation. The goal is not the cheapest solution at all cost. A higher cost may be tolerated if greater deliver speed can be achieved.

-   Identify possible sources of waste such as resources and resources with low usage rates

-   Right-size resources, such a virtual-machines, by analyzing performance metrics. Move to smaller instances when possible.

-   Use cloud providers' cost optimization services to review recommendations and decide whether to act upon them

-   Rely on horizontal scaling to increase resources during peak periods.

-   Align capacity and demand using elasticity of horizontal and vertical scaling

-   Turn off resources not used outside of core hours such as development and testing environments.

-   Analyze usage patterns to identify opportunity to migrate to reserved instances to achieve cost efficiencies

-   Use service with greater ability to reduce pay-per-use costs. For example, moving from virtual machines to serverless platforms will provide greater cost granularity, but also consider the cost of refactoring may nullify those cost efficiencies gained.

## References

-   Cloud FinOps: Collaborative, Real-Time Cloud Financial Management by J.R. Storment and Mike Fuller

-   <https://aws.amazon.com/aws-cost-management/aws-cost-optimization/>

-   Maximize Business Value with Cloud FinOps, Google Cloud, https://services.google.com/fh/files/blogs/cloud_finops_paper.pdf

## Automation

-   Report on the number of features requests in product backlogs are related to cost optimization.

-   Automate the periodic decommissioning of resources for development and testing environments outside of hours they are being used, for example, core hours.

-   Report on the number of compute instance and storage provisioned and trends over time.

# 07 Remediation
 

## Objectives

When cloud costs grow beyond forecasts, implement an action plan to analyze current usage and reduce waste.

## Description of Activities

When unplanned spend grows, implement a plan to remediate spending growth:

-   Report on unexpected cost growth to governance

-   Present an action plan to governance for addressing unexpected cost growth

-   Obtain authority from governance to execute on an action plan to remediate unexpected cost growth

-   Bring together implicated stakeholders to form a tiger team

-   Hold blameless retrospectives as a method of learning from accidental cost overruns with the intent to improve future practices rather than focus on assigning blame

-   Perform basic analysis. Determine the source of unplanned spend increases

-   Trace back spend growth to the source business activities

-   Set achievable targets for targets for spend reduction. Look for opportunities to reduce waste and optimize usage

-   Implement spend reduction activities

## References

-   Cloud Cost Optimization, Gartner, Mike Brown

-   Maximize Business Value with Cloud FinOps, Google Cloud, <https://services.google.com/fh/files/blogs/cloud_finops_paper.pdf>

-   <https://newrelic.com/blog/best-practices/blameless-retrospectives>

#08 Governance


## Objectives

Design and implement a governance to review and act upon cloud cost analysis

## Description of Activities

-   Encourage cloud cost transparency through reporting, including:

    -   Costs by provider and by product

    -   Shared costs

    -   Spend against budgets and forecasts

    -   Trends over time

    -   Top and low performing delivery teams/products in terms of cost optimization

-   Create processes for monitoring and taking corrective action, but without impacting the speed of delivery and agility of cloud

-   Decide on financial guardrails and alerting all delivery teams and products must adhere to

-   Cost governance does not require a dedicated governance vertical, but may be integrated into other governance activities such as performance, architecture, and security

-   Document the roles and responsibilities associated with cloud cost management

-   Favor guardrails over gates for enforcing policy

## References

-   Cloud FinOps: Collaborative, Real-Time Cloud Financial Management by J.R. Storment and Mike Fuller

-   <https://aws.amazon.com/blogs/enterprise-strategy/introducing-finops-excuse-me-devsecfinbizops/>

# 09 Business Metrics


## Objectives

Increased digitization of services and automation will drive up cloud costs over time that no amount of optimization efforts will be able to reverse. Business owners need to be explained cloud costs in terms of the business being delivered using cloud services. Delivery teams must be able to report on cloud costs in the context of business metrics. The unit economics, i.e., the cost per unit, must be calculated and reported.

## Description of Activities

-   Collaborate with business owners to understand their digital service deliver metrics (e.g., number of inquiries, wait times, number of transactions, speed of transactions, timeliness of transactions, total value of transactions, cost effectiveness, etc\...)

-   Report on cloud costs in terms of digital service delivery metrics (e.g., the average cost of serving an inquiry is X dollars)

-   Express technology investments in terms of service deliver metrics improvements (e.g., increased investment will result in increased ability to serve more inquiries)

-   Report on cost and digital service delivery metrics trends over time

## References

-   Cloud FinOps: Collaborative, Real-Time Cloud Financial Management by J.R. Storment and Mike Fuller

-   <https://aws.amazon.com/blogs/aws-cloud-financial-management/unit-metrics-in-practice-lessons-learned/>

# Cases Studies

## Treasury Board Secretariat -- Optimization with Reserved Instances

Treasury Board Secretariat migrated its entire portfolio of 120 plus applications to the cloud in 2020. In that time they have gain considerable experience with optimizing their cloud usage. Moving to Reserved Instances was one way TBS optimized its use of Virtual Machines. By lock-in to a three-year purchase of VMs, a 60%, or greater, savings was achieved over pay-as-you-go models (PAYG). TBS has calculated, that in most circumstances, the break even point of a reserved instance is 15 months. This means that even if the VM is only used for 15 months of the 36 total purchase period, cost savings occur over a PAYG model. For TBS, who automated the scheduled shut-down and start-up of development and test environments to save money, moving to RIs has achieved greater cost savings than scheduling and with lower complexity.

Next to migrating to reserved instances, TBS has also found setting and executing log retention periods are a considerable source of savings. Setting a retention policy for logs and then periodically cleaning up those logs that have exceeded the retention policy from block storage and PaaS yields cost avoidance.

## Canada Revenue Agency -- Budget, Allocation, Payment

The Canada Revenue Agency (CRA) has assembled a cross-functional FinOps using stakeholders from their Cloud Business Office (CBO) and Financial Advisory Services. This team undertakes the work of forecasting, budgeting, and tracking actual expenses.

![][1]

The process of forecasting, allocation, and payment at CRA is described as follows:

1.  Annually, the Cloud Business Office (CBO) forecasts the spend for Azure and AWS, with a breakdown per Cloud Business Requirement. Adjustments are made during the year based on need, avoiding Q4 when possible

2.  CBO makes a request to Central IT for commitment (funds added to requisition/order in CRA's SAP system)

3.  IT Contracting puts in place the Cloud Brokering Service Orders per Cloud Business Requirement selecting the Pay-as-you-go model (i.e. you get invoiced for what you use, no upfront costs or purchase commitments)

4.  Monthly invoices are reconciled and paid from Central IT's budget

5.  Finance charges back actual costs to business owners as per cost allocation tagging, plus the 10% Cloud Brokering Service. An internal transfer of funds is recovered to Central IT

Notes:

1.  Chargebacks are quarterly starting at P3 and then monthly in Q4

2.  FY-end funding transfer cut-off constraint: midway through March, finance forecasts the anticipated spend for charging back, risk managing the delta

3.  Shared Costs chargeback model is being developed in 2022

![][2]

## Statistics Canada -- Finops Organization

When Statistics Canada committed to migrating its application portfolio to cloud, they underwent a large change management not only in technology, but also in governance and practices. Part of that was investing in FinOps and establishing a FinOps organization. Statcan brings together people from the financial and technology organizations to monitor, management, and optimize cloud spend.

![][3]

## Canada Revenue Agency -- FinOps Training

When CRA began its FinOps journey, they wanted to provide the opportunity to stakeholders from technology and finance to understand FinOps practices. The [FinOps Foundation][4] is the learning provider they turned to for increasing organizational learning

![][5]


## Statistics Canada -- FinOps Reporting

To enable departmental monitoring and governance over cloud spend, StatCan has invested in tailored dashboards and reporting to attribute costs back to lines of business and fund centres.

![][6]

[^1]: Delivery Team refers to a multi-disciplinary team responsible for delivering a product using cloud. Deliver Team is used to denote the shift from organizing as functional silos towards multi-disciplinary teams made up of developers who build and run the product, architects, security, product managers, and user interface experts.

  [FinOps Foundation]: https://www.finops.org
  [1]: media/image1.png {width="6.5in" height="3.65625in"}
  [2]: media/image3.png {width="6.5in" height="3.65625in"}
  [3]: media/image5.png {width="5.921875546806649in" height="3.331055336832896in"}
  [4]: file:///C:\Users\MBEGIN\AppData\Local\Microsoft\Windows\INetCache\Content.Outlook\BOXMJH3I\finops-org.skilljar.com
  [5]: media/image7.png {width="6.5in" height="2.0833333333333335in"}
  [6]: media/image8.png {width="6.125in" height="3.4453127734033244in"}




<a name="francais"></a>Guide sur la gestion des coûts de l'informatique en nuage du gouvernement du Canada
-----------------------------------------------------------------------------------

# Objet

Le présent document vise à effectuer ce qui suit :

-   Soutenir l'adoption de l'infonuagique par les organisations du gouvernement du Canada tout en exerçant une diligence raisonnable sur le plan financier et en conservant une certaine souplesse;

-   Définir un ensemble de pratiques permettant d'assurer la gestion des coûts dans l'environnement infonuagique sans nuire à l'agilité et aux autres attributs du nuage;

-   Fournir aux parties prenantes un aperçu de la gestion des coûts de l'infonuagique, y compris les agents financiers et les agents d'approvisionnement.

# Contexte

L'informatique en nuage se base sur des modèles de paiement à vue et par répartition pour l'informatique, le stockage, le réseau, les plateformes et les solutions opérationnelles. Les coûts de l'infonuagique sont fluides et directement liés au prix unitaire des ressources multiplié par l'utilisation (coût = prix x utilisation). Il s'agit d'un changement fondamental par rapport aux modèles de consommation informatique traditionnels et fixes où le coût principal est associé à l'acquisition de matériel ou à l'octroi de licences de logiciels. Dans un modèle infonuagique, le coût constitue un facteur direct de l'architecture des applications. Les dépenses en infonuagique sont beaucoup plus dynamiques que celles dans les modèles de TI traditionnels, car les changements à l'utilisation entraînent des changements de coût immédiats. Il s'ensuit une boucle de rétroaction immédiate entre l'utilisation et coût. Les contrôles traditionnels des dépenses s'appuient fortement sur des contrôles au niveau du processus avec une surveillance exigeante en ressources humaines. Ces pratiques traditionnelles ne conviennent pas à un environnement infonuagique, car elles peuvent avoir une incidence négative sur l'agilité souhaitée par les équipes de livraison lors de l'utilisation du nuage et abaisser la valeur opérationnelle. Bien que les agents des finances et d'approvisionnement ne soient pas les gardiens des dépenses liées au nuage, ils aident les équipes de livraison à fixer le budget pour la livraison de leurs produits. Les équipes de livraison sont directement responsables des coûts du nuage et doivent être prêtes à suivre, analyser et optimiser les coûts associés à leurs produits et découlant de leur utilisation. Ces pratiques sont souvent appelées « OpFin ». Les OpFin sont un ensemble de pratiques qui favorisent la gestion et l'optimisation des dépenses dans le nuage sans nuire à l'agilité et à la rapidité de la prestation des services infonuagiques.

# OpFin

Souvent, le terme « OpFin » est appliqué à la gestion des coûts du nuage. Le terme est un mot-valise formé à partir des mots « opérations » et « financières ». La pratique est soutenue par la [Fondation des OpFin], une fondation dirigée par la collectivité. La fondation et les consultants en technologies ont construit et ont publié une banque de renseignements sur ce sujet. Le présent guide ne doit pas être lu isolément de cette banque de renseignements. Les OpFin constituent un domaine qui évolue au même rythme que le nuage.

# Comparaison des modèles traditionnels avec le modèle infonuagique

On peut penser au passage des modèles de TI traditionnels à un modèle infonuagique en utilisant l'analogie du passage du creusement et de l'entretien de son propre puits à la connexion au réseau municipal d'alimentation en eau. Les deux servent de sources d'approvisionnement en eau, mais chacune a un modèle sous-jacent différent. Dans le cas d'un puits, vous devez assumer la responsabilité de l'achat de l'équipement, de l'ingénierie et de la construction du puits, en plus de veiller à l'entretien des pompes et à la qualité de l'eau. Dans le cas d'un réseau municipal d'alimentation en eau, on vous facture simplement le service en fonction de la consommation mensuelle indiquée sur votre compteur d'eau et vous êtes abstrait des actifs nécessaires à la livraison de l'eau. Ce principe n'est pas tellement différent de celui du changement qu'a entraîné le modèle infonuagique. Les modèles informatiques traditionnels, tout comme le creusement de puits, constituent un modèle de livraison à forte intensité de capital et d'actifs. En revanche, le modèle infonuagique, tout comme l'approvisionnement en eau municipal, transforme l'approvisionnement informatique en un service primaire.

Dans le tableau ci-dessous, on suppose que le modèle à la carte dans le nuage est maintenu. Il convient de noter que selon la façon dont votre organisation établit la structure de son accord avec les fournisseurs, certaines parties de ce tableau peuvent ne pas s'appliquer. Par exemple, si un contrat oblige le consommateur à payer à l'avance pour des années de services, certaines des exigences énoncées dans ce tableau ne s'appliqueront pas. De plus, la portée de ce tableau est les services infonuagiques eux-mêmes et n'inclut pas les coûts en capital pour la mise en œuvre ou l'extension des services ou la construction de ces derniers à l'intérieur de ces plateformes.

| Modèles de TI traditionnels|Modèles infonuagiques|
|----------------------------|---------------------|
|Les services de TI traditionnels reposent sur un modèle de dépenses en capital où les biens (les logiciels, les matériels et les installations) sont achetés et conservés comme des actifs pendant une durée de vie déterminée.| Le service infonuagique est une dépense d'exploitation, tout comme un service public tel que l'électricité ou l'eau municipale, où les coûts varient en fonction du niveau d'utilisation.|
|Le niveau de consommation d'un actif (matériel et logiciel) n'a pas d'incidence importante sur le coût. Une fois que l'actif est acheté, les coûts sont irrécupérables et il n'existe aucun mécanisme pour optimiser ces coûts après que l'achat a été fait.|La consommation de ressources infonuagiques entraîne des coûts. La désactivation de l'utilisation d'un service permet de réaliser des économies de coûts.|
|Les investissements dans les modèles traditionnels sont généralement périodiques et sont associés au remplacement des biens vieillissants.| Les coûts des modèles infonuagiques sont à perpétuité jusqu'à la désactivation du service.|
|Les modèles traditionnels ont des coûts fixes.|Les coûts des modèles infonuagiques sont variables.|
|L'établissement de rapports sur les coûts des modèles traditionnels a lieu de façon périodique, souvent sur une base annuelle, car les coûts sont en grande partie fixes. |Les coûts des modèles infonuagiques sont en temps réel, car ils sont variables|
|Les modèles traditionnels ont un facteur de coût simple.|L'établissement des coûts des modèles infonuagiques est complexe et est souvent composé de microtransactions permettant de suivre chaque utilisation.|
|L'achat d'immobilisations est géré de manière centralisée par les organisations financières et d'approvisionnement.| Les achats des services infonuagiques sont décentralisés et sont effectués par les équipes de livraison fournissant des produits numériques à l'aide du nuage.|


# Optimiser les coûts du nuage

Si on le compare aux modèles de TI traditionnels, le modèle infonuagique offre plus d'options pour façonner les dépenses. Des leviers de décisions portant sur l'optimisation peuvent être utilisés pour réduire le gaspillage et déterminer la consommation appropriée. À l'inverse, des décisions peuvent être prises pour dépenser plus afin d'obtenir une plus grande vitesse et faciliter le déploiement. On peut produire une représentation graphique des choix d'optimisation sur un quadrant simple pour illustrer les compromis qui doivent être faits au chapitre du temps et du coût, comme le montre la figure 2. L'optimisation est axée sur la réduction du gaspillage et le contrôle des dépenses. L'optimisation continue peut ne pas entraîner de réduction des dépenses globales dans le nuage à long terme. Souvent, les organisations continuent d'augmenter leur utilisation du nuage avec le temps sous la forme de nouveaux services, de nouvelles données et de nouvelles expériences utilisateur. La numérisation accrue des activités d'une organisation entraînera, au fil du temps, une augmentation globale des dépenses liées au nuage. L'optimisation peut aider à assurer que les dépenses sont bien gérées et qu'elles n'entraînent pas de gaspillage inutile.

## Boucles de rétroaction

L'un des attributs clés de la gestion des coûts dans le modèle infonuagique dépend de la boucle de rétroaction en temps réel entre l'utilisation du nuage et les coûts du nuage. Cette simple boucle de rétroaction favorise l'adoption de comportements financiers permettant d'optimiser l'utilisation du nuage pour réduire les dépenses inutiles.

## Optimisation de la valeur opérationnelle, non la réduction au minimum des coûts

L'objectif de la gestion des coûts ne vise pas à réduire au minimum les coûts, mais plutôt à :

1.  réduire le gaspillage;

2.  permettre une offre de la valeur opérationnelle.

La réduction au minimum des coûts peut avoir une incidence sur la valeur opérationnelle. Les équipes de livraison et les propriétaires d'entreprise peuvent être prêts à faire des compromis et à payer des coûts plus élevés pour être en mesure d'assurer une livraison plus rapide. Par exemple, il se peut qu'une équipe de livraison opte pour le déploiement d'une architecture qui n'est pas optimisée tout simplement parce qu'une architecture plus simple peut permettre une livraison plus rapide d'une solution. Les compromis qui sont faits entre les économies pouvant être générées et l'effort nécessaire à la réalisation de ces économies sont illustrés ci-dessous. Un autre exemple est la priorité accordée au lancement d'une nouvelle fonctionnalité au détriment d'un autre affacturage d'un morceau de code qui pourrait entraîner une baisse des coûts du nuage. Par conséquent, l'optimisation des coûts fait partie intégrante des éléments de carnet d'un produit. Les possibilités d'optimiser un produit pour réduire les coûts doivent être hiérarchisées avec d'autres éléments de carnet d'un produit, comme l'ajout de nouvelles expériences utilisateur, l'application de nouvelles règles et l'inclusion d'autres demandes de fonctionnalités.

La gestion des coûts du nuage ne vise pas à réduire les coûts au minimum, mais plutôt à réaliser une vérification diligente sur le plan financier tout en améliorer la valeur commerciale pour l'organisation.

# Rôles

Ce document présente les rôles que doivent jouer les organisations pour exercer une diligence raisonnable à l'égard des dépenses liées au nuage. Il ne vise pas à fournir un ensemble exhaustif de pratiques, mais plutôt à décrire les pratiques minimales suggérées.

  |no.|role|
  |---|-----|
  |01|Responsabilité|
  |02|Visibilité et transparence|
  |03|Attribution des coûts|
  |04|Budgétisation|
  |05|Politiques sur les services et alertes|
  |06|Optimisation|
  |07|Limitation des coûts|
  |08|Gouvernance|
  |09|Définition des paramètres opérationnels|


# 01 Responsabilité


## Objectif

Les équipes de livraison[^1] doivent être prêtes à assumer des responsabilités quant à la gestion et à l'optimisation des coûts. Les répercussions des conceptions architecturales et des choix d'approvisionnement doivent être comprises par les membres de l'équipe de livraison.

## Description des activités

-   Veiller à ce que les équipes de livraison connaissent les conséquences de leurs décisions en matière de consommation, de configuration et d'architecture sur les coûts

-   Envisager de définir une exigence de formation sur la gestion financière dans le nuage (OpFin) pour tous les membres de l'équipe de livraison

-   S'assurer que les concepts de base des pratiques des OpFin et les garde-fous énumérés dans ce document soient compris par les membres de l'équipe de livraison

-   Utiliser l'approche RACI (responsable, agent comptable, consulté et informé) des OpFin du gouvernement du Canada (lien requis) comme modèle pour l'adapter aux rôles de votre organisation

-   Déterminer un rôle centralisé au sein de votre organisation qui gérera les données liées au nuage et les décisions relatives à la structure de gouvernance de votre organisation. Il ne s'agit pas nécessairement d'un rôle confié au centre d'expertise en infonuagique, mais fait plutôt partie de ses responsabilités.

-   Déterminer le rôle des agents financiers dans les pratiques des OpFin de votre organisation.

## Références

-   <https://finops.world/en/organization-and-key-roles/>

-   <https://finops.world/en/practices/card/1s1-assign-the-2-first-roles/>

# 02 Visibilité et transparence


## Objectif

Permettre aux équipes de livraison d'accéder librement aux rapports sur les coûts. Les équipes de livraison doivent avoir une vue complète sur les services et l'utilisation qui entraînent à l'augmentation des coûts des services infonuagiques associés à la livraison de leurs produits. Être transparent auprès de toutes les parties prenantes au sujet des coûts des services infonuagiques.

## Description des activités

-   Fournir des rapports et des tableaux de bord sur les dépenses passées, actuelles et prévues relatives aux services infonuagiques aux intervenants

-   Fournir des rapports de coûts standardisés à toutes les équipes de livraison, mais permettre aux équipes de livraison d'adapter ces rapports à leurs besoins

-   Fournir des rapports de manière à ce qu'une équipe de livraison puisse isoler les coûts associés à la livraison de ses produits

-   Maintenir la visibilité de tous les comptes et services infonuagiques. Si votre organisation a recours aux services infonuagiques de plusieurs fournisseurs, la visibilité de l'ensemble des fournisseurs et des comptes devra être assurée.

-   Offrir à tous les intervenants une transparence quant aux coûts des services infonuagiques.

-   Fixer la limite des dépenses de l'organisation associées aux services infonuagiques. Par exemple, le dirigeant principal de l'information ou le dirigeant principal des finances s'intéressent-ils aux rapports mensuels?

## Références

-   Cloud FinOps: Collaborative, Real-Time Cloud Financial Management by J.R. Storment and Mike Fuller

## Automatisation

-   Vérifier que le tableau de bord ou l'interface de protocole d'application (API) de facturation est utilisé sur une base périodique

-   Vérifier que le développeur et l'architecte ont également accès à la console et aux API de facturation

# 03 Attribution des coûts

## Objectif

Établir une structure pour l'étiquetage des ressources infonuagiques et l'attribution des coûts aux secteurs d'activité et aux centres de coûts qui financent ces coûts.

## Description des activités

-   Consigner et approuver un ensemble normalisé de balises pour identifier comment le coût des ressources est attribué aux applications et aux secteurs d'activité aux fins de facturation.

-   Consigner et approuver une structure hiérarchique des ressources ou des regroupements qui prennent en charge l'attribution des coûts aux secteurs d'activité aux fins de facturation.

-   Utiliser l'étiquetage et les structures des ressources pour assurer des possibilités de rapport supplémentaires afin que les coûts puissent être attribués aux secteurs d'activité et aux centres de financement qui financent la livraison des produits.

-   Rechercher et corriger toutes les ressources non étiquetées ou les ressources qui existent en dehors des structures de répartition des coûts.

-   Maintenir l'hygiène en matière des ressources :

    -   Identifier et corriger les ressources orphelines;

    -   Utiliser l'automatisation lors de la mise en œuvre de politiques de service pour appliquer les normes d'hygiène en matière de balisage dans la mesure du possible.

-   Pour les ressources de la plateforme infonuagique commune qui ne peuvent pas être attribuées à un seul produit ou secteur d'activité :

    -   Établir une méthode d'attribution des coûts communs, par exemple :

        -   Proportionnelle : basée sur le pourcentage relatif des coûts directs (par exemple, 10 % des dépenses directes relatives aux services infonuagiques);

        -   À parts égales : montant total réparti de façon égale entre les produits (par exemple, en divisant les coûts communs par le nombre de produits);

        -   Fixe : semblable à l'attribution à parts égales, mais en y incluant un coefficient pour pondérer la proportion allouée à chaque produit. La somme de tous les coefficients doit être 1 (par exemple, 0,3 des coûts communs).

    -   Déterminer une méthodologie de facturation ou de rétrofacturation pour rendre les coûts communs visibles pour chaque produit.

## Références

-   https://aws.amazon.com/blogs/aws-cloud-financial-management/cost-allocation-basics-that-you-need-to-know/

-   Cloud FinOps: Collaborative, Real-Time Cloud Financial Management by J.R. Storment and Mike Fuller

## Automatisation

-   Vérifier les ressources qui n'ont pas de balises approuvées de répartition des coûts.

-   Utiliser des règles de service pour appliquer les balises de répartition des coûts obligatoires.

# 04 Budgétisation



## Objectifs

Les équipes de livraison établissent les budgets des produits en collaboration avec les agents financiers et entreprennent des activités pour suivre les coûts réels par rapport aux prévisions.

## Description des activités

-   L'équipe de livraison travaillera avec les agents financiers pour établir un budget pour leur produit en fonction de l'estimation des coûts de l'hébergement dans les nuages.

-   Les budgets doivent être ventilés par période de facturation. Des alertes doivent être mises en place pour informer les équipes de livraison lorsqu'un pourcentage prédéterminé du budget mensuel prévu est dépensé.

-   Les équipes de livraison doivent rapporter les chiffres réels par rapport aux prévisions pour déterminer si le temps d'absorption correspond aux prévisions.

-   La gouvernance doit être documentée pour inclure le processus et les critères pour accroître les budgets.

-   La gouvernance du budget doit permettre une utilisation et des coûts imprévus, mais également prévoir des mesures correctives pour aider les équipes de livraison à gérer les dépenses imprévues répétitives.

## Références

-   Cloud FinOps: Collaborative, Real-Time Cloud Financial Management by J.R. Storment and Mike Fuller

-   https://aws.amazon.com/blogs/aws-cloud-financial-management/beginners-guide-to-aws-cost-management/

-   <https://docs.aws.amazon.com/cost-management/latest/userguide/budgets-create.html>

## Automatisation

-   Vérifier que les fonctionnalités des fournisseurs de services infonuagiques ont été configurées pour établir des budgets et envoyer des alertes sur ces derniers.

# 05 Politique et alertes


## Objectifs

Utiliser des alertes pour lancer des signaux d'alerte précoces lorsque des jalons financiers clés sont atteints, tels que le pourcentage des dépenses par rapport au budget total. Utiliser des politiques de service pour appliquer des garde-fous financiers clés tels que le respect des normes de balisage.

## Description

-   Utiliser la capacité des plateformes infonuagiques à alerter les utilisateurs des événements financiers comme méthode permettant d'automatiser les activités de gouvernance.

-   Utiliser des politiques de service pour faire respecter les principaux garde-fous financiers tels que le balisage et l'automatisation de la désactivation des services, en particulier pour les environnements de test et de développement. Les garde-fous financiers diffèrent des mesures de protection du nuage du gouvernement du Canada, car ils sont propres à chaque ministère et axés sur la gouvernance financière.

## Références

-   Cloud FinOps: Collaborative, Real-Time Cloud Financial Management by J.R. Storment and Mike Fuller

-   <https://cloud.google.com/billing/docs/how-to/budgets>

-   <https://docs.microsoft.com/en-us/azure/cost-management-billing/costs/cost-mgt-alerts-monitor-usage-spending>

-   <https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/monitor_estimated_charges_with_cloudwatch.html>

## Automatisation

-   Configurer des alertes pour les comptes ou les groupes de ressources afin d'informer les membres de l'équipe de livraison lorsque 25 %, 50 % et 75 % (ou toute autre valeur convenant à votre contexte) des ressources du budget total de l'équipe ont été consommées.

-   Définir des alertes en cas de variations excessives en pourcentage des coûts survenant sur une courte période.



# 06 Optimisation


## Objectifs

Les équipes de livraison doivent analyser continuellement les occasions pour optimiser l'utilisation et les architectures des services afin de réaliser des économies de coûts. Les équipes centralisées des OpFin peuvent cerner des possibilités d'optimisation pour aider les équipes de livraison à prendre des décisions d'optimisation.

## Description des activités

-   Les équipes de livraison examineront les rapports sur les coûts et de facturation pour cerner des possibilités d'optimisation et identifier les sources de gaspillage.

-   Elles compareront les avantages et les coûts de la mise en œuvre des stratégies d'optimisation

-   Les possibilités d'optimisation des architectures et de l'utilisation doivent être ajoutées au carnet de fonctionnalités du produit pour être priorisées aux côtés des demandes de fonctionnalités des utilisateurs et de la remédiation de la dette technique. L'objectif n'est pas de trouver la solution la moins chère à tout prix. Une solution plus chère peut être tolérée si elle peut permettre une plus grande vitesse de livraison.

-   Identifier les sources possibles de gaspillage telles que les ressources ayant un faible taux d'utilisation.

-   Adapter les ressources, telles que les machines virtuelles, en analysant les paramètres de rendement. Limiter les ressources utilisées dans la mesure du possible.

-   Utiliser les services d'optimisation des coûts des fournisseurs infonuagiques pour examiner les recommandations et décider sur l'exécution de ces recommandations.

-   S'appuyer sur la mise à l'échelle horizontale pour augmenter les ressources pendant les périodes de pointe.

-   Aligner la capacité et la demande en utilisant l'élasticité de la mise à l'échelle horizontale et verticale.

-   Désactiver les ressources qui ne sont pas utilisées en dehors des heures régulières, comme les environnements de développement et de test.

-   Analyser les modèles d'utilisation pour cerner les possibilités de passer aux instances réservées pour réaliser des économies de coûts.

-   Utiliser le service offrant une plus grande possibilité de réduire les coûts à l'utilisation. Par exemple, même si le passage des machines virtuelles aux plateformes sans serveur offrira une plus grande granularité des coûts, il faut également compte tenir compte du fait que le coût de la refactorisation qui peut annuler les économies de coûts réalisées.

## Références

-   Cloud FinOps: Collaborative, Real-Time Cloud Financial Management by J.R. Storment and Mike Fuller

-   <https://aws.amazon.com/aws-cost-management/aws-cost-optimization/>

-   Maximize Business Value with Cloud FinOps, Google Cloud, https://services.google.com/fh/files/blogs/cloud_finops_paper.pdf

## Automatisation

-   Rendre compte du nombre de demandes de fonctionnalités dans les carnets de produits qui sont liées à l'optimisation des coûts.

-   Automatiser la mise hors service périodique des ressources pour les environnements de développement et de test en dehors des heures d'utilisation, par exemple, les heures de base.

-   Rendre compte du nombre d'instances de calcul et de stockage provisionnées et des tendances au fil du temps.

# 07 Limitation des coûts

## Objectifs

Lorsque les coûts liés à l'infonuagique dépassent ce qui avait été prévu, il faut mettre en œuvre un plan d'action pour analyser l'utilisation actuelle et réduire le gaspillage.

## Description des activités

Lorsque les dépenses imprévues augmentent, les équipes doivent mettre en œuvre un plan pour limiter la croissance des dépenses :

-   Rendre compte de la croissance inattendue des coûts au Comité de gouvernance;

-   Présenter un plan d'action au Comité de gouvernance pour faire face à la croissance inattendue des coûts;

-   Demander l'autorisation du Comité de gouvernance pour exécuter un plan d'action pour remédier à la croissance inattendue des coûts;

-   Rassembler les intervenants impliqués pour former une équipe spéciale;

-   Effectuer des examens rétrospectifs sans blâme comme méthode d'apprentissage des dépassements de coûts accidentels dans le but d'améliorer les pratiques futures au lieu de blâmer;

-   Effectuer une analyse de base. Déterminer la source des augmentations de dépenses imprévues;

-   Retracer la croissance des dépenses aux activités commerciales sources;

-   Fixer des objectifs réalisables pour la réduction des dépenses. Cerner les occasions de réduire le gaspillage et d'optimiser l'utilisation des ressources;

-   Mettre en place des activités de réduction des dépenses.

## Références

-   Cloud Cost Optimization, Gartner, Mike Brown

-   Maximize Business Value with Cloud FinOps, Google Cloud, https://services.google.com/fh/files/blogs/cloud_finops_paper.pdf

-   <https://newrelic.com/blog/best-practices/blameless-retrospectives>

# 08 Gouvernance



## Objectifs

Concevoir et introduire un cadre de gouvernance pour examiner l'analyse des coûts du modèle infonuagique et adopter les mesures qui s'imposent, le cas échéant.

## Description des activités

-   Accroître la transparence des coûts du nuage en rendant compte, notamment :

    -   des coûts par fournisseur et par produit;

    -   des coûts partagés;

    -   des dépenses par rapport aux budgets et aux prévisions;

    -   des tendances au fil du temps;

    -   des équipes de livraison et des produits les plus performants et les moins performants en ce qui concerne l'optimisation des coûts.

-   Créer des processus de surveillance et de prise de mesures correctives sans nuire la rapidité de livraison ni à la souplesse des ressources infonuagiques.

-   Décider des garde-fous financiers et des produits que doivent respecter toutes les équipes de livraison et leur en aviser.

-   La gouvernance des coûts ne nécessite pas une structure de gouvernance verticale dédiée, mais peut être intégrée à d'autres activités de gouvernance telles que la performance, l'architecture et la sécurité.

-   Documenter les rôles et responsabilités associés à la gestion des coûts du nuage.

-   Favoriser les garde-fous au détriment des points de contrôle pour faire respecter les exigences de la politique.

## Références

-   Cloud FinOps: Collaborative, Real-Time Cloud Financial Management by J.R. Storment and Mike Fuller

-   <https://aws.amazon.com/blogs/enterprise-strategy/introducing-finops-excuse-me-devsecfinbizops/>

# 09 Paramètres opérationnels


## Objectifs

La numérisation et l'automatisation accrues des services augmenteront les coûts du nuage au fil du temps, une augmentation qui ne pourra être renversée par aucun effort d'optimisation. Les coûts des services infonuagiques en termes des activités pouvant être réalisées à l'aide de ces services doivent être expliqués aux propriétaires d'entreprise. Les équipes de livraison doivent être en mesure de rendre compte des coûts des services infonuagiques dans le contexte des mesures opérationnelles. Les aspects économiques unitaires, notamment le coût unitaire, doivent être calculés et déclarés.

## Description des activités

-   Collaborer avec les propriétaires d'entreprise pour comprendre leurs mesures de prestation de services numériques (par exemple, le nombre de demandes de renseignements, les temps d'attente, le nombre de transactions, la rapidité des transactions, le délai d'exécution des transactions, la valeur totale des transactions, la rentabilité, etc.).

-   Rendre compte des coûts du nuage en termes de paramètres de prestation de services numériques (par exemple, le coût moyen pour répondre à une demande est de X dollars).

-   Exprimer les investissements technologiques en termes de l'amélioration aux mesures de prestation de service (par exemple, une augmentation de l'investissement accru se traduira par une capacité accrue à répondre à un plus grand nombre de demandes).

-   Rendre compte des tendances des coûts et des paramètres de prestation de services numériques au fil du temps.

## Références

-   Cloud FinOps: Collaborative, Real-Time Cloud Financial Management by J.R. Storment and Mike Fuller

-   <https://aws.amazon.com/blogs/aws-cloud-financial-management/unit-metrics-in-practice-lessons-learned/>

# Cas d'utilisation

## Secrétariat du Conseil du Trésor du Canada -- Optimisation à l'aide des instances réservées

Le Secrétariat du Conseil du Trésor du Canada (SCT) a migré l'intégralité de son portefeuille de plus de 120 applications vers le nuage en 2020. Au cours de cette période, il a acquis une expérience considérable dans l'optimisation de son utilisation du nuage. Le passage aux instances réservées était l'un des moyens par lequel le SCT a optimisé son utilisation des machines virtuelles. La décision d'acheter des machines virtuelles sur une période de trois ans a permis de réaliser des économies de 60 % ou plus comparativement aux modèles à la carte. Le SCT a calculé que, dans la plupart des cas, une instance réservée atteint le seuil de rentabilité après 15 mois. Cela signifie que même si la machine virtuelle n'est utilisée que pendant 15 mois sur la période totale d'achat de 36 mois, des économies de coûts sont réalisées comparativement à un modèle à la carte. Pour le SCT, qui a automatisé l'arrêt et le démarrage programmés des environnements de développement et de test pour économiser de l'argent, le passage aux instances réservées a permis de réaliser davantage d'économies comparativement à la planification et avec un niveau de complexité moindre.

Outre la migration vers des instances réservées, le SCT a également constaté que la définition et l'exécution des périodes de conservation des registres permettent d'importantes économies. La définition d'une politique sur la conservation des registres et le nettoyage périodique subséquent des registres qui ont dépassé la période limite pour le stockage des blocs et des plateformes en tant que service permettent d'éviter des coûts.

## Agence du revenu du Canada -- Budget, allocation, et paiement

L'Agence du revenu du Canada (ARC) a assemblé une solution OpFin interfonctionnelle en utilisant les intervenants de son bureau d'affaires infonuagique et des services consultatifs en gestion financière. Cette équipe entreprend le travail de prévision, de budgétisation et de suivi des dépenses réelles.

![][2]

Le processus d'établissement des prévisions, d'affectation et de paiement à l'ARC est décrit comme suit :

1.  Chaque année, le bureau des opérations des services infonuagiques prévoit les dépenses pour Azure et Amazon Web Services (AWS), avec une ventilation par exigence opérationnelle infonuagique. Des ajustements sont effectués au cours de l'année en fonction des besoins, en évitant le quatrième trimestre lorsque cela est possible.

2.  Le bureau des opérations des services infonuagiques fait une demande d'engagement au service informatique central (pour ajouter des fonds à la demande et passage de la commande dans le système SAP de l'ARC).

3.  L'équipe de la passation de contrats de TI met en place les commandes de service de courtage infonuagique par exigence commerciale infonuagique en sélectionnant le modèle de paiement à l'utilisation (c'est-à-dire, que vous ne payez que pour les services que vous utilisez, sans avoir à payer de frais initiaux ni d'engagement d'achat).

4.  Les factures mensuelles sont réconciliées et payées à partir du budget des services de TI centraux.

5.  Le service des finances refacture les coûts réels aux propriétaires d'entreprise selon la répartition des coûts, en y incluant un supplément de 10 % pour le service de courtage infonuagique. Un transfert de fonds interne est effectué vers l'organisation centrale de TI.

Notes :

1.  Les refacturations sont effectuées sur une base trimestrielle à partir du T3, puis sur une base mensuelle à compter du T4.

2.  Contrainte d'arrêt des transferts de financement de fin d'exercice : à la mi-mars, le service des finances effectue la prévision des dépenses pour la refacturation et la gestion du risque delta.

3.  Le modèle de refacturation des coûts partagés est en cours d'élaboration en 2022.

![][3]

## Statistique Canada -- Organisation OpFin

Lorsque Statistique Canada s'est engagé à migrer son portefeuille d'applications vers le nuage, il a subi une importante gestion du changement non seulement sur le plan de la technologie, mais aussi en ce qui concerne la gouvernance et les pratiques. Une partie de cela consistait à investir dans les OpFin et à créer une organisation OpFin. Statcan regroupe des gens de différentes organisations financières et technologiques pour surveiller, gérer et optimiser les dépenses liées à l'infonuagique.

![][4]

## Agence du revenu du Canada -- Formation sur les OpFin

Lorsque l'ARC a commencé son parcours des OpFin, elle souhaitait offrir aux intervenants des secteurs de la technologie et des finances la possibilité de comprendre les pratiques des OpFin. La [Fondation des OpFin][5] est le fournisseur des services de formation vers lequel elle s'est tournée pour accroître l'apprentissage organisationnel.

![][6]


## Statistique Canada -- Rapports des OpFin

Pour assurer le contrôle et la gouvernance ministériels des dépenses liées aux services infonuagiques, StatCan a investi dans des tableaux de bord et des rapports personnalisés pour attribuer les coûts aux secteurs d'activité et aux centres de financement.

![][7]

[^1]: L'équipe de livraison fait référence à une équipe multidisciplinaire responsable de la livraison d'un produit à l'aide du nuage. Le terme « équipe de livraison » est utilisé pour désigner le passage d'une organisation en silos fonctionnels vers des équipes multidisciplinaires composées de développeurs qui élaborent et qui exécutent le produit, d'architectes, de responsables de la sécurité, de chefs de produit et d'experts de l'interface utilisateur.

  [Fondation des OpFin]: https://www.finops.org
  [1]: media/image1.png {width="0.4111111111111111in" height="0.4111111111111111in"}
  [2]: media/image3.png {width="6.5in" height="3.65625in"}
  [3]: media/image5.png {width="6.5in" height="3.65625in"}
  [4]: media/image7.png {width="5.921875546806649in" height="3.331055336832896in"}
  [5]: file:///C:\Users\MBEGIN\AppData\Local\Microsoft\Windows\INetCache\Content.Outlook\BOXMJH3I\finops-org.skilljar.com
  [6]: media/image9.png {width="6.5in" height="2.0833333333333335in"}
  [7]: media/image10.png {width="6.125in" height="3.4453127734033244in"}


