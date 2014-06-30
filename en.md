# Learning Measurement for Analytics Whitepaper

## Opportunity

The online educational landscape continues to yield significant growth in online digital curriculum development, delivery and enrollment. There is also a continued heightened interest in, and now demand for, accountability regarding the ability to measure and analyze this enriched online learning activity.  This interest, coupled with the more recent surge of the MOOCs and other online-only program offerings driving highly scaled online curriculum delivery, has caused the edtech ecosystem to explore and motivate a call to action to apply “Big Data” Analytics to education to drive a more efficient and informed online learning environment.  All of this attention on,and demand for,accountability backed by measurability, presents a very timely opportunity for IMS and standards to take a leadership position in defining a common foundation to enable the measurement of learning activity and its performance at a very granular level.

Equipped with a standards based common foundation for learning measurement, the quality,efficacy and performance derived analytics for the online curriculum across the ecosystem can be achieved more effectively.  Both the producers (i.e. institutions, instructors, curriculum developers, learning designers,etc.) and consumers (i.e. learners/students) of this online curriculum can better engage, measure, revise,and iterate to foster a much more informed continuous improvement of the curriculum and the learning experience outcomes.  In addition, institutions as well as,edtech solution providers can deliver the high-demand/high-value, new and enhanced data driven extensions to the online learning delivery platform such as learning analytics, predictive analytics/pathing, adaptive learning, personalization, early warningalerts, badging/certification, etc.

Given this timely and high value opportunity scenario, some of the key challenges identified that need to be prioritized and factored into a strategy and direction to realize a learning measurement standards-based framework are:

- In the current state of online curriculum delivery, there are a non-standard and/or completely non-existent set of metrics for measuring curriculum learning activity content and feature-function edu-apps, sourced from an increasingly wider spectrum of solutions and providers.  This diverse solution set is highly federated, fragmented and ‘siloed’within the provider’srespective delivery platform/app.  These collections ofsolutions frequentlyco-exist in any given online lesson or curriculum. Some progress is being made in establishing some learning design/objective performance oriented standardized metrics (i.e. [Bloom’s Taxonomy], [Common Core], [Predictive Analytics Reporting (PAR) framework][PAR], [Council for the Advancement of Standards in Higher Education -Learning and Developmental Outcomes][CAS standards]) but have yet to be more universally applied and/or leveraged within a broader context of measurements;

[Bloom’s Taxonomy]: http://en.wikipedia.org/wiki/Bloom's_Taxonomy

[Common Core]: http://www.corestandards.org/the-standards

[PAR]: https://public.datacookbook.com/public/institutions/par

[CAS standards]: http://www.cas.edu/index.php/cas-general-standards/

- Given this state, it is difficult to establish a unified and consistent view of measured learning activity within and across curriculum, independent of the delivery context;
- It is difficult to effectively compare,contrast, and correlate learning activity, determine the efficacy of curriculum, and evaluate learner interaction and the potential impact on performance without a standardized and consistent instrumentation framework and set of metrics;
- Substantial pre-existing work e.g.Learning Tools Interoperability™(LTI)™, Learning Information Services (LIS), Question and Test Interoperability™(QTI)™has been done to standardize the learning activity encapsulation and context that can be leveraged, but it needs to be extended to engage learning measurement;
- There have been manyoverlapping and partial emerging conventions and standards stemming from the fast emerging broad spectrum of Big Data technologies and Data Science initiatives. These technologies and initiatives contain, no, early stage or yet-to-be-determined applicability to online education optimized measurement and analytics standardizatione.g. NoSQL, cloud-scale Relational Databases, Graph Databases, Map-Reduce, ADL Experience/TinCan API, etc.

While embracing this opportunity and its challenges, it is important to recognize and factor in the potential leverage of a fast emerging collection of foundational data science related methodologies, standards and technologies as selective elements of a model that can apply to an education optimized application targeting learning measurement.This can serve to deliver not only great efficiency,butalso drive standardization across verticals wherever possible, andexpedite the design, implementation and scale of an educational vertical applied solution.

In addition, it is important to recognize that the “edu graph” (depicted in Figure1) of education associated measurement and data  (akin to the “social graph” of social data that has emerged), can be expandedin both breadth and depth across multiple areas of specialized data contexts associated withinthe ecosystemand theeducational workflow contextualized sources of data such as administrative/operational, curricular activity and content, co-curricular, learner/educator profile, career,etc.

**Figure 1: The comprehensive “edu graph” data mode**

*With that, it is important to befocused,initially,on a smaller subset of the edu-graph so as to achieve the impact and value of the resulting enhanced learning measurement, while establishing a standardized software services framework that can be readily applied and extended toincrementally cover the other facets of the edu-graph over time.*

The proposed focus put forward in this white paper targets the “learning graph” facets of the broader edu-graph thatintentionally targets the critical curriculum learning activity and associated efficacy and performance measurement.  The rationale for choosing this initial learning graph focus area is simple: to target the actual learning context that is at the epicenter of the overall educational workflow and from which measurement of all other contexts can extend and add further insight and value.

## Strategic Direction

The strategy described in this whitepaper is intended to provide a high-level recommendation of how Learning Systems should capture and share data around learning interactions, using existing and upcoming IMS specifications, that can be used to support and advance Learning Measurement and Analytics.

*It is important to note that the focus and initial priority of this strategy is primarily on bringing order via a standardized Measurement framework to enable the more comprehensive Learning Analytics domain of solutions.*

IMS and standards can play the much needed instrumental role in first establishinga strong foundation to consistently represent, capture, and marshalmeasurement related data, which willthen set the stage of a whole ecosystem of higher-order analytics solutions that canbe greatly enabled and enhanced.

In order to further this goal, IMS will work with its member institutions and suppliers to define aLearning Measurement Framework -**Caliper**.  This framework is depicted in Figure 2.

*Note that the scope of Caliper is denoted in Figure 2 by the left-hand, shaded green box.*

**Figure 2:IMS Caliper -Learning Measurement Framework**

MS Caliper is built around the following concepts:

- **IMS Learning Metric Profiles** that provide a Learning Activity centric focus to standardize on metrics (actions and related context) captured across consumerandproducer learning tool’s deliveryactivities and deliveryplatforms that consumeand orchestrateactivity based curriculum, while providing for custom extensions and future additions to the profiles;
- **IMS Learning Sensor API** and Learning Eventsdrivestandardized instrumentation and metric capture and marshal between tools and their delivery platforms and/or associated analytics service solution aggregating metrics;
- **IMS LTI™/LIS/QTI™ leverage and extensionsen** hance and integrate granular, standardized learning measurement with tools interoperability and the underlying learning information models, inclusive of course, learner, outcomes and other critical associated context.The following sections describe the elements of the framework in greater detail.

### IMS Learning Activity Metric Profiles

The learning curriculum is typically composed and delivered as a collection,or sequence,of one or more Learning Activities.  Most Learning Activities can be grouped into one (or more, in the case of composite activities) genres -e.g.Reading, Assessment, Media, Collaboration,etc.  This helps to organize and optimize measurements for each specific genre of Learning Activity to begin to baseline consistent metrics.

IMS Learning Metric Profiles are intended to define a standardized, structured collection of **Learning Activity Metrics** that represent granular **measurements** specific to **actions** within each genre of **activity** including all relevant **context** for any given action on an activity.  In addition, there are pan-genre **Foundational Metrics** such as **engagement**, performance, etc., that support common measurement of more generally applicable metrics across all activities.  Any given Learning Activity can have (one or more) Metric Profiles associated with it to collect and exchange whatever measurements whichneed to captured and managed.

IMS has work ongoing to define an initial set of Learning Metric Profiles for the most common Learning Activity types, that will be a used as a component of,or extensions to, current and/or in-process/future planned IMS standards, like LTI™, LISand QTI™, etc.  These IMS standardsspecify the contextual elements (information model) against which metrics will be captured.  Together the Activity metrics and information models will define metric profiles, i.e. provide a base “schema”, that will allow for a standards-based measurement and exchange of learning data between systems.

Figure 3 depicts a sample (non-definitive) of the types of Metric Profiles that IMS intends to develop in collaboration with its member institutions and suppliers.

**Figure 3: IMS Metric Profiles -Sample**

The IMS Learning Analytics group will leverage and incorporate, into the Caliper Metrics Profiles, ongoing efforts by various organizations to define metrics and/or desired learning and developmental outcomes for various aspects of the edu-graph. These include (but are not limited to):

- [The Predictive Analytics Reporting (PAR) framework’s][PAR] Data Models as part of IMS Context and Engagement metrics;
- [Common Core Standards][Common Core] as part of IMS Performance metrics;
- [CAS standards for student developmental and learning outcomes for higher education][CAS standards] as part of IMS Performancemetrics.

### IMS Learning Sensor API and Learning Events

Closely tied to the **Learning Activity Metric Profiles**, the **IMS Sensor API** is intended to support the instrumentation, collection and exchange of data from Learning Tools/Systems and associated Learning Content elements. This will enable the availability of standard metrics accessed via any given Analytics Store and associated APIs.

At its core, the **Sensor API** will support the exchange of **Learning Events** based on interactions with/on Learning Activities.  As depicted in Figure3, Learning Events will be expressed in the form of a data triple **-“LearningContext” -“Action” -“ActivityContext”**.  This is based on the W3C RDF Triple form of "subject/predicate/object" -i.e. an expression linking one object (subject) to another object(object) or a literalvia a predicate.  In this case, the Learning Event will allow for the expression of the measurement of an interaction with a Learning Activity.

Learning Events will be consumed by **Sensor endpoints**.These can be implemented by any application that wishes to consume Learning Events and is expected to support popular protocols like HTTP/REST.

**Figure 4: IMS Sensor API -Learning Event**

The way to visualize this is to start with the **LearningContext**. A Learning Context is basically the environment in which teaching and learning occurs. This can include a Course, Instructor, Student, Learning Platform, Program, Institution, etc.

Learning **Activities** are introduced into the LearningContext to facilitate teaching and learning. These Activities typically include Readings, Videos, Quizzes, Discussions, etc. Activities are typically grouped and sequenced into a prescribed learning path.

Finally, in the process of teaching and learning, there are interactions between entities in LearningContext and Activities. We call these **Actions**.

The combination of these three data sets into a **LearningEvent** is intended to completely describe an interactionwith an Activity within a LearningContext. In addition to the three data sets in the triple, each LearningEvent is timestamped.

As depicted in Figure 4, each element of the Learning Event triple defines one or more of the entities in a learning interaction.  Together, these entities make up the **Learning Graph** based on the connectedness of the entities within a learning environment. Each of these elements will be further described based on existing IMS specificationsand vocabulary,as well as,the in-progress IMS Learning Activity Metric profiles.

The Learning Events and Metric Profiles are intended to strike a balance between a completely open mechanism and a rigid schema for measuring and analyzing learning in the scope of the Learning Graph.  The Metric Profiles are intended to apply a very lightweight schema while allowing for marshaling of custom data specific to a particular App/System with a goal of enhancing the profiles in a very iterative way in order to support the needs of the EdTechcommunity.

This mechanism also allowsfor existing “open” triple based API’s to be mapped and marshaled over the Sensor API and for any such existing “open” API’s to consume Learning Events based on IMS Activity Metric Profiles.  One such example is the Experience/TinCan API.  Caliper’s Sensor API and the Experience API share a common foundation with regard to communicating data via triples.  The IMS Caliper framework,however,is more encompassing of the ecosystem in that it:

- Takes a learning environment specific view via Learning Metric Profiles;
- Includes LTI™-as an important component of the framework/specification;
- Incorporates existing specifications/standards fordata interoperability like LIS, QTI™, etc.
- Will strive to incorporate ongoing effortsby various organizations to define metrics and/or desired learning and developmental outcomes for various aspects of the edu-graph.

Note that the two can be interoperable, in that:

- IMS Learning Events can be consumed by a TinCanLRS via the generic subject-verb-object transport;
- TinCan triples can be consumed byanIMS Sensor API (this requires mapping to Learning Activity Metric Profiles -something that should be completed before any useful analysis can be undertakenon TinCan triples).

However, it should be noted that leverage of something like a TinCan enabled event handling framework is completely optional,as the Caliper Sensor API provides intrinsic capabilities for the capture and marshaling of learning events to route to a target analytics store.  An integration mapping with Caliper Learning Events should only be necessary if TinCan is leveraged as a low-level event transport across a much broader set of tracking contexts inclusive of learning activity.


### IMS Learning Tools Interoperability and Learning Information ServicesExtensions

The IMS Learning Tools Interoperability™(LTI) specification is one of the most widelyused and successful interoperability mechanisms in the Ed Tech space today.  It enables Learning Systems and Tools to provide an integrated learning experience to Instructors, Course Designers,and Learners.  While the current version of LTI allows for seamless operational integration, the learning data generated is still isolated to each individual tool participating the in the LTI integration.In addition to the Metric Profiles and the Sensor API/Learning Events, IMS intends to define extensions so that:

- LTI tools can specify one or more metric profiles in their LTI descriptor;
- LTI consumers as part of the LTI handshake can specify IMS Sensor API end-point to which the tools can push data conforming to the metric profiles during tool usage.

Figure 5 depicts the intended scope of the extensions (highlighted in red) to the LTI framework.

**Figure 5: IMS LTI Extensions to support Measurement Framework**

As a result of these extensions, LTI Consumer and Tools will be able to exchange data in accordance with the Metric Profiles using the Sensor API.

Ongoing IMS work will seek to bridge and extend the LIS outcomes work to not only the proposed LTI extension,but also to cover any omissionsintroduced via Caliper.For example, efforts to define and incorporate a methodology to represent and authorize/resolve any parameterized event context such as a unique person ID associated with an action, will be factored into follow-on specification and framework workgroup initiatives.

## Applied Scenario

This section outlines a scenario applying all of the elements of IMS Caliper. It is important to note that the IMS member organizations will continue to collaborate on realizing this framework in the near-term.Figure 6 depicts the scenario.  As shown, the entities involved are:

- A Learning Platform that supports **LTI**;
- Two **LTI Apps** that contribute a Reading and Video Activity respectively to a course in the LMS.  The LTI Apps both support the **IMS Learning Activity Metric Profile** for their genreand **Sensor API** and are able to send **Learning Events** to a Sensor **endpoint**;
- An **Analytics Service** that supports the IMS Sensor API. The Analytics Service also provides a Analytics Dashboardto the Learning Platform.

**Figure 6: Applied Scenario for IMS Learning Analytics Measurement Framework**

The following is the sequence of events for this scenario:

- The Learning PlatformAdministrator configures two LTI Apps.  The LTI configuration URL/XML indicates to the Learning Platformthat these Apps support a Reading and Video Metric Profile respectively. *Note that with LTI v2 (currently in public draft), the LTI App/Tool configuration can be automated via a REST API implemented by the interacting consumer/tool.  As a result, LTI configuration is greatly simplified.  In addition, the Sensor Endpoint URL configuration described below could also be included in the Tool Proxy Registration flow defined as part of LTI v2;*
- The Learning PlatformAdministrator configures the Sensor API Endpoint URL in the LTI settings.  This is a URL provided by the Analytics Service.  The URL could possibly have an embedded API Key authorizing access;
- An Instructor adds a Reading and Video Activity using the LTI Apps
    * In order to add the two activities, the Instructor initiatesan LTI launch.  During the launch, since the Apps support IMS Metric Profiles, the LMS adds on the Sensor API Endpoint URL as one of the launch parameters
    * The App receives the Sensor API Endpoint as part of the launch and stores this for future use;
- A Student starts accessing a course in the Learning Platformand as part of the assignmentsbeginsusing the Reading and Video.  During this use, the student performs several typical actions, such as:
    * Reading a page
    * Highlighting a section
    * Adding a Bookmark
    * Viewing the video
    * Taking a note on the Video at a particular time during playback;
- The LTI Apps record the student’sactions.  Since the Learning Platform provided a Sensor API endpoint during launch, each App starts posting Learning Events to the Sensor API endpoint;
- The Analytics Service
    * Is a proxy for a typical consuming service for metrics captured and marshaled via the IMS Caliper framework. Note that the Analytics Service and any associated services such as the access and store interfaces and stack, areoutside the scope of the IMS Caliper framework from a standards based framework perspective
    * Records the Learning Events to its store
    * Supports and provides more detailed analysis of the metrics to yield higher order functionality such as dashboards, recommendations/alerts, adaptive sequencing etc.
    * Providers for Analytics Services include, butarenot limited to many of the LMS suppliers, adaptive learning suppliers, predictive analytics suppliers,etc.
    * Depicted in the Analytics Dashboard delivered via an LMS is just one example of such value. Additional functionality leveraging Learning Measurement Framework could potentially be encapsulated as an LTI app and easily be delivered in other app contexts.


## Conclusion and Recommendations

The IMS Caliper Learning Measurement Framework represents a valuable, standards oriented, high impact solution to a very significant problem amidst the online learning delivery ecosystem. Currently, this ecosystemhas an insufficient, inconsistent, and fragmented underlying measurement and metrics capability across a fast emerging of federated content/learning activity elements sourced from a wide array of providers.  By providing the necessary alignment and structure to what is and should be measured, along with aframework to support the capture and marshaling, this IMS Caliper focused scope represents an achievableand valuable starting position.

Clearly, the Caliper framework is flexible and extendable which willgreatly facilitate the recommended and likely iterative build-out, refinement, and enhancement of its capabilities.In addition, the framework could addother adjacent complementary analytics frameworks, as time and the solution-space evolves. This proposed solution simply establishes a direction and scope to drive value.

An additionaldetailed definition, specificationand supporting service framework implementation will be forthcomingas the IMS workgroup roadmaps and tasks are prioritized.  This work willdrive getting the integral and co-dependent work done in respective IMS workgroups (i.e. Learning Analytics, LTI, LIS, QTI,etc.) to both support and realize the implementation of the Caliper interdependent elements, and more importantly, synchronize around a more unified, consistent and standardized approach to learning measurement.

## Appendix A -Glossary

<table>
<thead>
<tr>
<th>Term</th><th>Description</th>
</tr>
<thead>
<tbody>
<tr>
<td>Caliper</td><td>The IMS Learning Measurement Framework providing a standardized representation, capture,and marshaling of learning activity generated metrics targeted for consumption by any conforming sensor API endpoint enabled analytics store/ services.</td>
</tr>
<tr>
<td>Edu Graph</td><td>Much like the social graph of data nodes, edges and elements across the vast social networking ecosystem of applications and users, the edu-graph represents the vast educational focused graph of data for the online education ecosystem.</td>
</tr>
<tr>
<td>Learning Activity</td><td>Any web content and/or edu App deliveringfeature-functionality (e.g. LTI tool) that encapsulates a single component of a learning sequence which is typically denoted as an lesson or curriculum.  Activities can be assignable and/or gradable as required.</td>
</tr>
<tr>
<td>Learning Event</td><td>Smallest element of measurement captured within the context of any learning activity that is represented as a journaled fact comprised of an activity context, an action, and an learning context.</td>
</tr>
<tr>
<td>Learning Graph</td><td>As a sub-graph of the Edu Graph data model, this graph data focuses on all learning centric granular, learning activity generated metrics associated with curriculum engagement, performance / efficacy and activity specific contextual measurement.</td>
</tr>
<tr>
<td>Learning Information Services (LIS)</td><td>Refer to the <a href="http://www.imsglobal.org/lis/">IMS Learning Information Services specification</a></td>
</tr>
<tr>
<td>Learning Tools Interoperability™ (LTI™)</td><td>Refer to the <a href="http://www.imsglobal.org/toolsinteroperability2.cfm">Learning Tools Interoperability specification</a></td>
</tr>
<tr>
<td>Metric Profile</td><td>Standardized collection of granular metrics that are both learning activity 
agnostic (i.e. engagement, performance, etc.) and learning activity genre 
specific (i.e. reading, quizzing, media, etc.). Profiles are utilized to capture and 
marshal metrics via the Caliper framework in a standardized consistent form. </td>
</tr>
<tr>
<td>Question and Test Interoperability™ (QTI™)</td><td>Refer to the <a href="">IMS Question & Test Interoperability specification</a></td>
</tr>
<tr>
<td>Sensor API</td><td>API that includes the Learning Event, inclusive of binding to the Metric Profiles, 
and the endpoints that consume these events.</td>
</tr>
</tbody>
</table>