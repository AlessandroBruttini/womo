Markdown documentation created by [pyLODE](http://github.com/rdflib/pyLODE) 2.4

# The Occupant-centric Workplace Management ontology (WOMO)

## Metadata

- **IRI**
  - `https://w3id.org/womo#`
- **Creators(s)**
  - [Alessandro Bruttini](https://orcid.org/0000-0001-6317-2406)
    [[ORCID]](https://orcid.org/0000-0001-6317-2406)
    (<alessandro.bruttini@unifi.it></a>) of [University of Florence, IT](https://www.linkedin.com/in/alessandro-bruttini-2228883b/)
- **Created**
  - 2023-07-19
- **Version Information**
  - 1.0
- **License**
  - CC-BY-40
- **Ontology RDF**
  - RDF ([.\womo.ttl](turtle))

### Description

<p>The Occupant-centric Workplace Management (WOMO) ontology describes knowledge related to office environments and enables the development of a workplace Digital Twin system centred on the occupant experience.</p>

## Table of Contents

1. [Classes](#classes)
1. [Object Properties](#objectproperties)
1. [Datatype Properties](#datatypeproperties)
1. [Named Individuals](#namedindividuals)
1. [Namespaces](#namespaces)
1. [Legend](#legend)

## Overview

![Womo ontology overview](womo.png "Womo ontology overview").
**Figure 1:** WOMO Ontology overview

## Classes

[Activity](#Activity),
[ActivityCategory](#ActivityCategory),
[ActivityType](#ActivityType),
[CommonSpace](#CommonSpace),
[Condition](#Condition),
[ConditionType](#ConditionType),
[Department](#Department),
[EnclosedOffice](#EnclosedOffice),
[Feedback](#Feedback),
[FeedbackGenerationType](#FeedbackGenerationType),
[FeedbackResponseType](#FeedbackResponseType),
[HealthIndicator](#HealthIndicator),
[HealthIndicatorType](#HealthIndicatorType),
[MechanicalVentilationControlType](#MechanicalVentilationControlType),
[Member](#Member),
[NaturalVentilationControlType](#NaturalVentilationControlType),
[NotRespondedFeedback](#NotRespondedFeedback),
[Office](#Office),
[Organization](#Organization),
[Preference](#Preference),
[RatingScale](#RatingScale),
[RespondedFeedback](#RespondedFeedback),
[Room](#Room),
[SocialInteraction](#SocialInteraction),
[VentilationType](#VentilationType),
[Worker](#Worker),
[WorkerFeature](#WorkerFeature),
[Workspace](#Workspace),
[WorkspaceElement](#WorkspaceElement),
[WorkspaceType](#WorkspaceType),
[Workstation](#Workstation),

### Activity

| Property      | Value                                                                                                                                                                                                                                                                                                                                                                              |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| IRI           | `https://w3id.org/womo#Activity`                                                                                                                                                                                                                                                                                                                                                   |
| Description   | <p>Thing that the worker is doing.</p>                                                                                                                                                                                                                                                                                                                                             |
| Super-classes | [owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />                                                                                                                                                                                                                                                                                                                         |
| In domain of  | [womo:hasActivityCategory](https://w3id.org/womo#hasActivityCategory) (op)<br />[womo:hasSocialInteraction](https://w3id.org/womo#hasSocialInteraction) (op)<br />[womo:isPerformedBy](https://w3id.org/womo#isPerformedBy) (op)<br />[womo:hasActivityType](https://w3id.org/womo#hasActivityType) (op)<br />[womo:isPerformedAt](https://w3id.org/womo#isPerformedAt) (op)<br /> |
| In range of   | [womo:isActivityCategoryOf](https://w3id.org/womo#isActivityCategoryOf) (op)<br />[womo:performs](https://w3id.org/womo#performs) (op)<br />[womo:isActivityTypeOf](https://w3id.org/womo#isActivityTypeOf) (op)<br />[womo:hasActivity](https://w3id.org/womo#hasActivity) (op)<br />[womo:isSocialInteractionOf](https://w3id.org/womo#isSocialInteractionOf) (op)<br />         |

### ActivityCategory

| Property      | Value                                                                              |
| ------------- | ---------------------------------------------------------------------------------- |
| IRI           | `https://w3id.org/womo#ActivityCategory`                                           |
| Description   | <p>Specifies the category of the activity that the worker is performing.</p>       |
| Super-classes | [owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />                         |
| In domain of  | [womo:isActivityCategoryOf](https://w3id.org/womo#isActivityCategoryOf) (op)<br /> |
| In range of   | [womo:hasActivityCategory](https://w3id.org/womo#hasActivityCategory) (op)<br />   |

### ActivityType

| Property      | Value                                                                                                                                                                  |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| IRI           | `https://w3id.org/womo#ActivityType`                                                                                                                                   |
| Description   | <p>Specifies the type of activity that the worker is performing.</p>                                                                                                   |
| Super-classes | [owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />                                                                                                             |
| In domain of  | [womo:isActivityTypeSupportedBy](https://w3id.org/womo#isActivityTypeSupportedBy) (op)<br />[womo:isActivityTypeOf](https://w3id.org/womo#isActivityTypeOf) (op)<br /> |
| In range of   | [womo:hasActivityType](https://w3id.org/womo#hasActivityType) (op)<br />[womo:supportsActivityType](https://w3id.org/womo#supportsActivityType) (op)<br />             |

### CommonSpace

| Property      | Value                                                               |
| ------------- | ------------------------------------------------------------------- |
| IRI           | `https://w3id.org/womo#CommonSpace`                                 |
| Super-classes | [womo:WorkspaceType](https://w3id.org/womo#WorkspaceType) (c)<br /> |

### Condition

| Property      | Value                                                                        |
| ------------- | ---------------------------------------------------------------------------- |
| IRI           | `https://w3id.org/womo#Condition`                                            |
| Super-classes | [womo:WorkerFeature](https://w3id.org/womo#WorkerFeature) (c)<br />          |
| In domain of  | [womo:hasConditionType](https://w3id.org/womo#hasConditionType) (op)<br />   |
| In range of   | [womo:isConditionTypeOf](https://w3id.org/womo#isConditionTypeOf) (op)<br /> |

### ConditionType

| Property      | Value                                                                        |
| ------------- | ---------------------------------------------------------------------------- |
| IRI           | `https://w3id.org/womo#ConditionType`                                        |
| Super-classes | [owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />                   |
| In domain of  | [womo:isConditionTypeOf](https://w3id.org/womo#isConditionTypeOf) (op)<br /> |
| In range of   | [womo:hasConditionType](https://w3id.org/womo#hasConditionType) (op)<br />   |

### Department

| Property      | Value                                                             |
| ------------- | ----------------------------------------------------------------- |
| IRI           | `https://w3id.org/womo#Department`                                |
| Super-classes | [womo:Organization](https://w3id.org/womo#Organization) (c)<br /> |

### EnclosedOffice

| Property      | Value                                                 |
| ------------- | ----------------------------------------------------- |
| IRI           | `https://w3id.org/womo#EnclosedOffice`                |
| Super-classes | [womo:Office](https://w3id.org/womo#Office) (c)<br /> |

### Feedback

| Property      | Value                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| IRI           | `https://w3id.org/womo#Feedback`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| Super-classes | [owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| In domain of  | [womo:hasFeedbackGenerationType](https://w3id.org/womo#hasFeedbackGenerationType) (op)<br />[womo:feedbackTime](https://w3id.org/womo#feedbackTime) (dp)<br />[womo:hasFeedbackResponseType](https://w3id.org/womo#hasFeedbackResponseType) (op)<br />[womo:feedbackRequestTime](https://w3id.org/womo#feedbackRequestTime) (dp)<br />[womo:isProvidedAt](https://w3id.org/womo#isProvidedAt) (op)<br />[womo:feedbackStartTime](https://w3id.org/womo#feedbackStartTime) (dp)<br />[womo:responseDuration](https://w3id.org/womo#responseDuration) (dp)<br />[womo:isProvidedBy](https://w3id.org/womo#isProvidedBy) (op)<br />[womo:reports](https://w3id.org/womo#reports) (op)<br />[womo:responseRatio](https://w3id.org/womo#responseRatio) (dp)<br /> |
| In range of   | [womo:isReportedBy](https://w3id.org/womo#isReportedBy) (op)<br />[womo:isFeedbackResponseTypeOf](https://w3id.org/womo#isFeedbackResponseTypeOf) (op)<br />[womo:provides](https://w3id.org/womo#provides) (op)<br />[womo:hasFeedback](https://w3id.org/womo#hasFeedback) (op)<br />[womo:isFeedbackGenerationTypeOf](https://w3id.org/womo#isFeedbackGenerationTypeOf) (op)<br />                                                                                                                                                                                                                                                                                                                                                                         |

### FeedbackGenerationType

| Property      | Value                                                                                          |
| ------------- | ---------------------------------------------------------------------------------------------- |
| IRI           | `https://w3id.org/womo#FeedbackGenerationType`                                                 |
| Description   | <p>Instances of this class enumerates possible feedback request generation types.</p>          |
| Super-classes | [owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />                                     |
| In domain of  | [womo:isFeedbackGenerationTypeOf](https://w3id.org/womo#isFeedbackGenerationTypeOf) (op)<br /> |
| In range of   | [womo:hasFeedbackGenerationType](https://w3id.org/womo#hasFeedbackGenerationType) (op)<br />   |

### FeedbackResponseType

| Property      | Value                                                                                                                                                        |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| IRI           | `https://w3id.org/womo#FeedbackResponseType`                                                                                                                 |
| Description   | <p>Instances of this class enumerates possible feedback response types.</p>                                                                                  |
| Super-classes | [owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />                                                                                                   |
| Sub-classes   | [womo:NotRespondedFeedback](https://w3id.org/womo#NotRespondedFeedback) (c)<br />[womo:RespondedFeedback](https://w3id.org/womo#RespondedFeedback) (c)<br /> |
| In domain of  | [womo:isFeedbackResponseTypeOf](https://w3id.org/womo#isFeedbackResponseTypeOf) (op)<br />                                                                   |
| In range of   | [womo:hasFeedbackResponseType](https://w3id.org/womo#hasFeedbackResponseType) (op)<br />                                                                     |

### HealthIndicator

| Property      | Value                                                                                                                                      |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| IRI           | `https://w3id.org/womo#HealthIndicator`                                                                                                    |
| Super-classes | [womo:WorkerFeature](https://w3id.org/womo#WorkerFeature) (c)<br />                                                                        |
| In domain of  | [womo:value](https://w3id.org/womo#value) (dp)<br />[womo:hasHealthIndicatorType](https://w3id.org/womo#hasHealthIndicatorType) (op)<br /> |
| In range of   | [womo:isHealthIndicatorTypeOf](https://w3id.org/womo#isHealthIndicatorTypeOf) (op)<br />                                                   |

### HealthIndicatorType

| Property      | Value                                                                                    |
| ------------- | ---------------------------------------------------------------------------------------- |
| IRI           | `https://w3id.org/womo#HealthIndicatorType`                                              |
| Super-classes | [owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />                               |
| In domain of  | [womo:isHealthIndicatorTypeOf](https://w3id.org/womo#isHealthIndicatorTypeOf) (op)<br /> |
| In range of   | [womo:hasHealthIndicatorType](https://w3id.org/womo#hasHealthIndicatorType) (op)<br />   |

### MechanicalVentilationControlType

| Property      | Value                                                                                                              |
| ------------- | ------------------------------------------------------------------------------------------------------------------ |
| IRI           | `https://w3id.org/womo#MechanicalVentilationControlType`                                                           |
| Super-classes | [owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />                                                         |
| In domain of  | [womo:isMechanicalVentilationControlTypeOf](https://w3id.org/womo#isMechanicalVentilationControlTypeOf) (op)<br /> |
| In range of   | [womo:hasMechanicalVentilationControlType](https://w3id.org/womo#hasMechanicalVentilationControlType) (op)<br />   |

### Member

| Property      | Value                                                          |
| ------------- | -------------------------------------------------------------- |
| IRI           | `https://w3id.org/womo#Member`                                 |
| Super-classes | [owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />     |
| Sub-classes   | [womo:Worker](https://w3id.org/womo#Worker) (c)<br />          |
| In domain of  | [womo:isMemberOf](https://w3id.org/womo#isMemberOf) (op)<br /> |
| In range of   | [womo:hasMember](https://w3id.org/womo#hasMember) (op)<br />   |

### NaturalVentilationControlType

| Property      | Value                                                                                                        |
| ------------- | ------------------------------------------------------------------------------------------------------------ |
| IRI           | `https://w3id.org/womo#NaturalVentilationControlType`                                                        |
| Super-classes | [owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />                                                   |
| In domain of  | [womo:isNaturalVentilationControlTypeOf](https://w3id.org/womo#isNaturalVentilationControlTypeOf) (op)<br /> |
| In range of   | [womo:hasNaturalVentilationControlType](https://w3id.org/womo#hasNaturalVentilationControlType) (op)<br />   |

### NotRespondedFeedback

| Property      | Value                                                                               |
| ------------- | ----------------------------------------------------------------------------------- |
| IRI           | `https://w3id.org/womo#NotRespondedFeedback`                                        |
| Description   | <p>Instances of this class enumerates possible types of not responded feedback.</p> |
| Super-classes | [womo:FeedbackResponseType](https://w3id.org/womo#FeedbackResponseType) (c)<br />   |

### Office

| Property      | Value                                                                 |
| ------------- | --------------------------------------------------------------------- |
| IRI           | `https://w3id.org/womo#Office`                                        |
| Super-classes | [womo:Room](https://w3id.org/womo#Room) (c)<br />                     |
| Sub-classes   | [womo:EnclosedOffice](https://w3id.org/womo#EnclosedOffice) (c)<br /> |

### Organization

| Property      | Value                                                                                                                                                                                                                                                                                                                                                                                                  |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| IRI           | `https://w3id.org/womo#Organization`                                                                                                                                                                                                                                                                                                                                                                   |
| Super-classes | [owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />                                                                                                                                                                                                                                                                                                                                             |
| Sub-classes   | [womo:Department](https://w3id.org/womo#Department) (c)<br />                                                                                                                                                                                                                                                                                                                                          |
| In domain of  | [womo:organizationLogo](https://w3id.org/womo#organizationLogo) (dp)<br />[womo:hasMember](https://w3id.org/womo#hasMember) (op)<br />[womo:isPartOf](https://w3id.org/womo#isPartOf) (op)<br />[womo:hasPart](https://w3id.org/womo#hasPart) (op)<br />[womo:organizationName](https://w3id.org/womo#organizationName) (dp)<br />[womo:ownsWorkspace](https://w3id.org/womo#ownsWorkspace) (op)<br /> |
| In range of   | [womo:hasPart](https://w3id.org/womo#hasPart) (op)<br />[womo:isWorkspaceOf](https://w3id.org/womo#isWorkspaceOf) (op)<br />[womo:isMemberOf](https://w3id.org/womo#isMemberOf) (op)<br />[womo:isPartOf](https://w3id.org/womo#isPartOf) (op)<br />                                                                                                                                                   |

### Preference

| Property      | Value                                                                    |
| ------------- | ------------------------------------------------------------------------ |
| IRI           | `https://w3id.org/womo#Preference`                                       |
| Super-classes | [womo:WorkerFeature](https://w3id.org/womo#WorkerFeature) (c)<br />      |
| In domain of  | [womo:isPreferenceFor](https://w3id.org/womo#isPreferenceFor) (op)<br /> |
| In range of   | [womo:isPreferredAs](https://w3id.org/womo#isPreferredAs) (op)<br />     |

### RatingScale

| Property      | Value                                                                                                                                                                                                                                                                                                      |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| IRI           | `https://w3id.org/womo#RatingScale`                                                                                                                                                                                                                                                                        |
| Super-classes | [owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />                                                                                                                                                                                                                                                 |
| In domain of  | [womo:ratingScalePrompt](https://w3id.org/womo#ratingScalePrompt) (dp)<br />[womo:ratingScaleName](https://w3id.org/womo#ratingScaleName) (dp)<br />[womo:ratingScaleOptions](https://w3id.org/womo#ratingScaleOptions) (dp)<br />[womo:isRatingScaleOf](https://w3id.org/womo#isRatingScaleOf) (op)<br /> |
| In range of   | [womo:hasRatingScale](https://w3id.org/womo#hasRatingScale) (op)<br />                                                                                                                                                                                                                                     |

### RespondedFeedback

| Property      | Value                                                                             |
| ------------- | --------------------------------------------------------------------------------- |
| IRI           | `https://w3id.org/womo#RespondedFeedback`                                         |
| Description   | <p>Instances of this class enumerates possible types of responded feedback.</p>   |
| Super-classes | [womo:FeedbackResponseType](https://w3id.org/womo#FeedbackResponseType) (c)<br /> |

### Room

| Property      | Value                                                               |
| ------------- | ------------------------------------------------------------------- |
| IRI           | `https://w3id.org/womo#Room`                                        |
| Super-classes | [womo:WorkspaceType](https://w3id.org/womo#WorkspaceType) (c)<br /> |
| Sub-classes   | [womo:Office](https://w3id.org/womo#Office) (c)<br />               |

### SocialInteraction

| Property      | Value                                                                                |
| ------------- | ------------------------------------------------------------------------------------ |
| IRI           | `https://w3id.org/womo#SocialInteraction`                                            |
| Super-classes | [owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />                           |
| In domain of  | [womo:isSocialInteractionOf](https://w3id.org/womo#isSocialInteractionOf) (op)<br /> |
| In range of   | [womo:hasSocialInteraction](https://w3id.org/womo#hasSocialInteraction) (op)<br />   |

### VentilationType

| Property      | Value                                                                            |
| ------------- | -------------------------------------------------------------------------------- |
| IRI           | `https://w3id.org/womo#VentilationType`                                          |
| Super-classes | [owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />                       |
| In domain of  | [womo:isVentilationTypeOf](https://w3id.org/womo#isVentilationTypeOf) (op)<br /> |
| In range of   | [womo:hasVentilationType](https://w3id.org/womo#hasVentilationType) (op)<br />   |

### Worker

| Property      | Value                                                                                                                                                                                                                                                                                  |
| ------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| IRI           | `https://w3id.org/womo#Worker`                                                                                                                                                                                                                                                         |
| Super-classes | [womo:Member](https://w3id.org/womo#Member) (c)<br />[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />                                                                                                                                                                        |
| In domain of  | [womo:hasWorkerFeature](https://w3id.org/womo#hasWorkerFeature) (op)<br />[womo:performs](https://w3id.org/womo#performs) (op)<br />[womo:hasAllocatedWorkspace](https://w3id.org/womo#hasAllocatedWorkspace) (op)<br />[womo:provides](https://w3id.org/womo#provides) (op)<br />     |
| In range of   | [womo:isWorkerFeatureOf](https://w3id.org/womo#isWorkerFeatureOf) (op)<br />[womo:isAllocatedTo](https://w3id.org/womo#isAllocatedTo) (op)<br />[womo:isProvidedBy](https://w3id.org/womo#isProvidedBy) (op)<br />[womo:isPerformedBy](https://w3id.org/womo#isPerformedBy) (op)<br /> |

### WorkerFeature

| Property      | Value                                                                                                                                                                                           |
| ------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| IRI           | `https://w3id.org/womo#WorkerFeature`                                                                                                                                                           |
| Super-classes | [owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />                                                                                                                                      |
| Sub-classes   | [womo:Condition](https://w3id.org/womo#Condition) (c)<br />[womo:HealthIndicator](https://w3id.org/womo#HealthIndicator) (c)<br />[womo:Preference](https://w3id.org/womo#Preference) (c)<br /> |
| In domain of  | [womo:isWorkerFeatureOf](https://w3id.org/womo#isWorkerFeatureOf) (op)<br />                                                                                                                    |
| In range of   | [womo:hasWorkerFeature](https://w3id.org/womo#hasWorkerFeature) (op)<br />                                                                                                                      |

### Workspace

| Property      | Value                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| IRI           | `https://w3id.org/womo#Workspace`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| Super-classes | [https://w3id.org/bot#Space](https://w3id.org/bot#Space) (c)<br />[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />[sosa:FeatureOfInterest](http://www.w3.org/ns/sosa/FeatureOfInterest) (c)<br />                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| In domain of  | [womo:workspaceVolumePerOccupant](https://w3id.org/womo#workspaceVolumePerOccupant) (dp)<br />[womo:supportsActivityType](https://w3id.org/womo#supportsActivityType) (op)<br />[womo:workspaceNetFloorArea](https://w3id.org/womo#workspaceNetFloorArea) (dp)<br />[womo:hasVentilationType](https://w3id.org/womo#hasVentilationType) (op)<br />[womo:isWorkspaceOf](https://w3id.org/womo#isWorkspaceOf) (op)<br />[womo:workspaceOccupancyNumber](https://w3id.org/womo#workspaceOccupancyNumber) (dp)<br />[womo:hasNaturalVentilationControlType](https://w3id.org/womo#hasNaturalVentilationControlType) (op)<br />[womo:workspacePubliclyAccessible](https://w3id.org/womo#workspacePubliclyAccessible) (dp)<br />[womo:workspaceHeight](https://w3id.org/womo#workspaceHeight) (dp)<br />[womo:isAllocatedTo](https://w3id.org/womo#isAllocatedTo) (op)<br />[womo:workspaceLocalID](https://w3id.org/womo#workspaceLocalID) (dp)<br />[womo:workspaceNetVolume](https://w3id.org/womo#workspaceNetVolume) (dp)<br />[womo:hasMechanicalVentilationControlType](https://w3id.org/womo#hasMechanicalVentilationControlType) (op)<br />[womo:workspaceAreaPerOccupant](https://w3id.org/womo#workspaceAreaPerOccupant) (dp)<br />[womo:hasFeedback](https://w3id.org/womo#hasFeedback) (op)<br />[womo:hasWorkspaceType](https://w3id.org/womo#hasWorkspaceType) (op)<br />[womo:workspaceIsShared](https://w3id.org/womo#workspaceIsShared) (dp)<br />[womo:hasWorkspace](https://w3id.org/womo#hasWorkspace) (op)<br />[womo:hasActivity](https://w3id.org/womo#hasActivity) (op)<br />[womo:containsWorkspaceElement](https://w3id.org/womo#containsWorkspaceElement) (op)<br /> |
| In range of   | [womo:isProvidedAt](https://w3id.org/womo#isProvidedAt) (op)<br />[womo:hasAllocatedWorkspace](https://w3id.org/womo#hasAllocatedWorkspace) (op)<br />[womo:hasWorkspace](https://w3id.org/womo#hasWorkspace) (op)<br />[womo:isNaturalVentilationControlTypeOf](https://w3id.org/womo#isNaturalVentilationControlTypeOf) (op)<br />[womo:isVentilationTypeOf](https://w3id.org/womo#isVentilationTypeOf) (op)<br />[womo:isMechanicalVentilationControlTypeOf](https://w3id.org/womo#isMechanicalVentilationControlTypeOf) (op)<br />[womo:isPerformedAt](https://w3id.org/womo#isPerformedAt) (op)<br />[womo:isWorkspaceTypeOf](https://w3id.org/womo#isWorkspaceTypeOf) (op)<br />[womo:isActivityTypeSupportedBy](https://w3id.org/womo#isActivityTypeSupportedBy) (op)<br />[womo:ownsWorkspace](https://w3id.org/womo#ownsWorkspace) (op)<br />                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |

### WorkspaceElement

| Property      | Value                                                                                                                                                                                                           |
| ------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| IRI           | `https://w3id.org/womo#WorkspaceElement`                                                                                                                                                                        |
| Super-classes | [owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />[https://w3id.org/bot#Element](https://w3id.org/bot#Element) (c)<br />[sosa:FeatureOfInterest](http://www.w3.org/ns/sosa/FeatureOfInterest) (c)<br /> |
| In domain of  | [womo:hasSubWorkspaceElement](https://w3id.org/womo#hasSubWorkspaceElement) (op)<br />                                                                                                                          |
| In range of   | [womo:containsWorkspaceElement](https://w3id.org/womo#containsWorkspaceElement) (op)<br />[womo:hasSubWorkspaceElement](https://w3id.org/womo#hasSubWorkspaceElement) (op)<br />                                |

### WorkspaceType

| Property      | Value                                                                                                                                                                           |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| IRI           | `https://w3id.org/womo#WorkspaceType`                                                                                                                                           |
| Super-classes | [owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />                                                                                                                      |
| Sub-classes   | [womo:Room](https://w3id.org/womo#Room) (c)<br />[womo:Workstation](https://w3id.org/womo#Workstation) (c)<br />[womo:CommonSpace](https://w3id.org/womo#CommonSpace) (c)<br /> |
| In domain of  | [womo:isWorkspaceTypeOf](https://w3id.org/womo#isWorkspaceTypeOf) (op)<br />                                                                                                    |
| In range of   | [womo:hasWorkspaceType](https://w3id.org/womo#hasWorkspaceType) (op)<br />                                                                                                      |

### Workstation

| Property      | Value                                                               |
| ------------- | ------------------------------------------------------------------- |
| IRI           | `https://w3id.org/womo#Workstation`                                 |
| Super-classes | [womo:WorkspaceType](https://w3id.org/womo#WorkspaceType) (c)<br /> |

## Object Properties

[containsWorkspaceElement](#containsWorkspaceElement),
[hasActivity](#hasActivity),
[hasActivityCategory](#hasActivityCategory),
[hasActivityType](#hasActivityType),
[hasAllocatedWorkspace](#hasAllocatedWorkspace),
[hasConditionType](#hasConditionType),
[hasFeedback](#hasFeedback),
[hasFeedbackGenerationType](#hasFeedbackGenerationType),
[hasFeedbackResponseType](#hasFeedbackResponseType),
[hasHealthIndicatorType](#hasHealthIndicatorType),
[hasMechanicalVentilationControlType](#hasMechanicalVentilationControlType),
[hasMember](#hasMember),
[hasNaturalVentilationControlType](#hasNaturalVentilationControlType),
[hasPart](#hasPart),
[hasRatingScale](#hasRatingScale),
[hasSocialInteraction](#hasSocialInteraction),
[hasSubWorkspaceElement](#hasSubWorkspaceElement),
[hasVentilationType](#hasVentilationType),
[hasWorkerFeature](#hasWorkerFeature),
[hasWorkspace](#hasWorkspace),
[hasWorkspaceType](#hasWorkspaceType),
[isActivityCategoryOf](#isActivityCategoryOf),
[isActivityTypeOf](#isActivityTypeOf),
[isActivityTypeSupportedBy](#isActivityTypeSupportedBy),
[isAllocatedTo](#isAllocatedTo),
[isConditionTypeOf](#isConditionTypeOf),
[isFeedbackGenerationTypeOf](#isFeedbackGenerationTypeOf),
[isFeedbackResponseTypeOf](#isFeedbackResponseTypeOf),
[isHealthIndicatorTypeOf](#isHealthIndicatorTypeOf),
[isMechanicalVentilationControlTypeOf](#isMechanicalVentilationControlTypeOf),
[isMemberOf](#isMemberOf),
[isNaturalVentilationControlTypeOf](#isNaturalVentilationControlTypeOf),
[isPartOf](#isPartOf),
[isPerformedAt](#isPerformedAt),
[isPerformedBy](#isPerformedBy),
[isPreferenceFor](#isPreferenceFor),
[isPreferredAs](#isPreferredAs),
[isProvidedAt](#isProvidedAt),
[isProvidedBy](#isProvidedBy),
[isRatingScaleOf](#isRatingScaleOf),
[isRelatedTo](#isRelatedTo),
[isReportedBy](#isReportedBy),
[isSocialInteractionOf](#isSocialInteractionOf),
[isVentilationTypeOf](#isVentilationTypeOf),
[isWorkerFeatureOf](#isWorkerFeatureOf),
[isWorkspaceOf](#isWorkspaceOf),
[isWorkspaceTypeOf](#isWorkspaceTypeOf),
[ownsWorkspace](#ownsWorkspace),
[performs](#performs),
[provides](#provides),
[reports](#reports),
[supportsActivityType](#supportsActivityType),
[](containsWorkspaceElement)

### containsWorkspaceElement

| Property         | Value                                                                              |
| ---------------- | ---------------------------------------------------------------------------------- |
| IRI              | `https://w3id.org/womo#containsWorkspaceElement`                                   |
| Super-properties | [https://w3id.org/bot#containsElement](https://w3id.org/bot#containsElement)<br /> |
| Domain(s)        | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br />                        |
| Range(s)         | [womo:WorkspaceElement](https://w3id.org/womo#WorkspaceElement) (c)<br />          |

[](hasActivity)

### hasActivity

| Property  | Value                                                       |
| --------- | ----------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#hasActivity`                         |
| Domain(s) | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br /> |
| Range(s)  | [womo:Activity](https://w3id.org/womo#Activity) (c)<br />   |

[](hasActivityCategory)

### hasActivityCategory

| Property  | Value                                                                     |
| --------- | ------------------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#hasActivityCategory`                               |
| Domain(s) | [womo:Activity](https://w3id.org/womo#Activity) (c)<br />                 |
| Range(s)  | [womo:ActivityCategory](https://w3id.org/womo#ActivityCategory) (c)<br /> |

[](hasActivityType)

### hasActivityType

| Property  | Value                                                             |
| --------- | ----------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#hasActivityType`                           |
| Domain(s) | [womo:Activity](https://w3id.org/womo#Activity) (c)<br />         |
| Range(s)  | [womo:ActivityType](https://w3id.org/womo#ActivityType) (c)<br /> |

[](hasAllocatedWorkspace)

### hasAllocatedWorkspace

| Property  | Value                                                       |
| --------- | ----------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#hasAllocatedWorkspace`               |
| Domain(s) | [womo:Worker](https://w3id.org/womo#Worker) (c)<br />       |
| Range(s)  | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br /> |

[](hasConditionType)

### hasConditionType

| Property  | Value                                                               |
| --------- | ------------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#hasConditionType`                            |
| Domain(s) | [womo:Condition](https://w3id.org/womo#Condition) (c)<br />         |
| Range(s)  | [womo:ConditionType](https://w3id.org/womo#ConditionType) (c)<br /> |

[](hasFeedback)

### hasFeedback

| Property  | Value                                                       |
| --------- | ----------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#hasFeedback`                         |
| Domain(s) | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br /> |
| Range(s)  | [womo:Feedback](https://w3id.org/womo#Feedback) (c)<br />   |

[](hasFeedbackGenerationType)

### hasFeedbackGenerationType

| Property  | Value                                                                                 |
| --------- | ------------------------------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#hasFeedbackGenerationType`                                     |
| Domain(s) | [womo:Feedback](https://w3id.org/womo#Feedback) (c)<br />                             |
| Range(s)  | [womo:FeedbackGenerationType](https://w3id.org/womo#FeedbackGenerationType) (c)<br /> |

[](hasFeedbackResponseType)

### hasFeedbackResponseType

| Property  | Value                                                                             |
| --------- | --------------------------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#hasFeedbackResponseType`                                   |
| Domain(s) | [womo:Feedback](https://w3id.org/womo#Feedback) (c)<br />                         |
| Range(s)  | [womo:FeedbackResponseType](https://w3id.org/womo#FeedbackResponseType) (c)<br /> |

[](hasHealthIndicatorType)

### hasHealthIndicatorType

| Property  | Value                                                                           |
| --------- | ------------------------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#hasHealthIndicatorType`                                  |
| Domain(s) | [womo:HealthIndicator](https://w3id.org/womo#HealthIndicator) (c)<br />         |
| Range(s)  | [womo:HealthIndicatorType](https://w3id.org/womo#HealthIndicatorType) (c)<br /> |

[](hasMechanicalVentilationControlType)

### hasMechanicalVentilationControlType

| Property  | Value                                                                                                     |
| --------- | --------------------------------------------------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#hasMechanicalVentilationControlType`                                               |
| Domain(s) | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br />                                               |
| Range(s)  | [womo:MechanicalVentilationControlType](https://w3id.org/womo#MechanicalVentilationControlType) (c)<br /> |

[](hasMember)

### hasMember

| Property  | Value                                                             |
| --------- | ----------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#hasMember`                                 |
| Domain(s) | [womo:Organization](https://w3id.org/womo#Organization) (c)<br /> |
| Range(s)  | [womo:Member](https://w3id.org/womo#Member) (c)<br />             |

[](hasNaturalVentilationControlType)

### hasNaturalVentilationControlType

| Property  | Value                                                                                               |
| --------- | --------------------------------------------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#hasNaturalVentilationControlType`                                            |
| Domain(s) | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br />                                         |
| Range(s)  | [womo:NaturalVentilationControlType](https://w3id.org/womo#NaturalVentilationControlType) (c)<br /> |

[](hasPart)

### hasPart

| Property  | Value                                                             |
| --------- | ----------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#hasPart`                                   |
| Domain(s) | [womo:Organization](https://w3id.org/womo#Organization) (c)<br /> |
| Range(s)  | [womo:Organization](https://w3id.org/womo#Organization) (c)<br /> |

[](hasRatingScale)

### hasRatingScale

| Property  | Value                                                                                                                    |
| --------- | ------------------------------------------------------------------------------------------------------------------------ |
| IRI       | `https://w3id.org/womo#hasRatingScale`                                                                                   |
| Domain(s) | ([womo:Condition](https://w3id.org/womo#Condition) (c) or [womo:Preference](https://w3id.org/womo#Preference) (c))<br /> |
| Range(s)  | [womo:RatingScale](https://w3id.org/womo#RatingScale) (c)<br />                                                          |

[](hasSocialInteraction)

### hasSocialInteraction

| Property  | Value                                                                       |
| --------- | --------------------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#hasSocialInteraction`                                |
| Domain(s) | [womo:Activity](https://w3id.org/womo#Activity) (c)<br />                   |
| Range(s)  | [womo:SocialInteraction](https://w3id.org/womo#SocialInteraction) (c)<br /> |

[](hasSubWorkspaceElement)

### hasSubWorkspaceElement

| Property         | Value                                                                          |
| ---------------- | ------------------------------------------------------------------------------ |
| IRI              | `https://w3id.org/womo#hasSubWorkspaceElement`                                 |
| Super-properties | [https://w3id.org/bot#hasSubElement](https://w3id.org/bot#hasSubElement)<br /> |
| Domain(s)        | [womo:WorkspaceElement](https://w3id.org/womo#WorkspaceElement) (c)<br />      |
| Range(s)         | [womo:WorkspaceElement](https://w3id.org/womo#WorkspaceElement) (c)<br />      |

[](hasVentilationType)

### hasVentilationType

| Property  | Value                                                                   |
| --------- | ----------------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#hasVentilationType`                              |
| Domain(s) | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br />             |
| Range(s)  | [womo:VentilationType](https://w3id.org/womo#VentilationType) (c)<br /> |

[](hasWorkerFeature)

### hasWorkerFeature

| Property  | Value                                                               |
| --------- | ------------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#hasWorkerFeature`                            |
| Domain(s) | [womo:Worker](https://w3id.org/womo#Worker) (c)<br />               |
| Range(s)  | [womo:WorkerFeature](https://w3id.org/womo#WorkerFeature) (c)<br /> |

[](hasWorkspace)

### hasWorkspace

| Property         | Value                                                                |
| ---------------- | -------------------------------------------------------------------- |
| IRI              | `https://w3id.org/womo#hasWorkspace`                                 |
| Super-properties | [https://w3id.org/bot#hasSpace](https://w3id.org/bot#hasSpace)<br /> |
| Domain(s)        | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br />          |
| Range(s)         | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br />          |

[](hasWorkspaceType)

### hasWorkspaceType

| Property  | Value                                                               |
| --------- | ------------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#hasWorkspaceType`                            |
| Domain(s) | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br />         |
| Range(s)  | [womo:WorkspaceType](https://w3id.org/womo#WorkspaceType) (c)<br /> |

[](isActivityCategoryOf)

### isActivityCategoryOf

| Property  | Value                                                                     |
| --------- | ------------------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#isActivityCategoryOf`                              |
| Domain(s) | [womo:ActivityCategory](https://w3id.org/womo#ActivityCategory) (c)<br /> |
| Range(s)  | [womo:Activity](https://w3id.org/womo#Activity) (c)<br />                 |

[](isActivityTypeOf)

### isActivityTypeOf

| Property  | Value                                                             |
| --------- | ----------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#isActivityTypeOf`                          |
| Domain(s) | [womo:ActivityType](https://w3id.org/womo#ActivityType) (c)<br /> |
| Range(s)  | [womo:Activity](https://w3id.org/womo#Activity) (c)<br />         |

[](isActivityTypeSupportedBy)

### isActivityTypeSupportedBy

| Property  | Value                                                             |
| --------- | ----------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#isActivityTypeSupportedBy`                 |
| Domain(s) | [womo:ActivityType](https://w3id.org/womo#ActivityType) (c)<br /> |
| Range(s)  | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br />       |

[](isAllocatedTo)

### isAllocatedTo

| Property  | Value                                                       |
| --------- | ----------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#isAllocatedTo`                       |
| Domain(s) | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br /> |
| Range(s)  | [womo:Worker](https://w3id.org/womo#Worker) (c)<br />       |

[](isConditionTypeOf)

### isConditionTypeOf

| Property  | Value                                                               |
| --------- | ------------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#isConditionTypeOf`                           |
| Domain(s) | [womo:ConditionType](https://w3id.org/womo#ConditionType) (c)<br /> |
| Range(s)  | [womo:Condition](https://w3id.org/womo#Condition) (c)<br />         |

[](isFeedbackGenerationTypeOf)

### isFeedbackGenerationTypeOf

| Property  | Value                                                                                 |
| --------- | ------------------------------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#isFeedbackGenerationTypeOf`                                    |
| Domain(s) | [womo:FeedbackGenerationType](https://w3id.org/womo#FeedbackGenerationType) (c)<br /> |
| Range(s)  | [womo:Feedback](https://w3id.org/womo#Feedback) (c)<br />                             |

[](isFeedbackResponseTypeOf)

### isFeedbackResponseTypeOf

| Property  | Value                                                                             |
| --------- | --------------------------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#isFeedbackResponseTypeOf`                                  |
| Domain(s) | [womo:FeedbackResponseType](https://w3id.org/womo#FeedbackResponseType) (c)<br /> |
| Range(s)  | [womo:Feedback](https://w3id.org/womo#Feedback) (c)<br />                         |

[](isHealthIndicatorTypeOf)

### isHealthIndicatorTypeOf

| Property  | Value                                                                           |
| --------- | ------------------------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#isHealthIndicatorTypeOf`                                 |
| Domain(s) | [womo:HealthIndicatorType](https://w3id.org/womo#HealthIndicatorType) (c)<br /> |
| Range(s)  | [womo:HealthIndicator](https://w3id.org/womo#HealthIndicator) (c)<br />         |

[](isMechanicalVentilationControlTypeOf)

### isMechanicalVentilationControlTypeOf

| Property  | Value                                                                                                     |
| --------- | --------------------------------------------------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#isMechanicalVentilationControlTypeOf`                                              |
| Domain(s) | [womo:MechanicalVentilationControlType](https://w3id.org/womo#MechanicalVentilationControlType) (c)<br /> |
| Range(s)  | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br />                                               |

[](isMemberOf)

### isMemberOf

| Property  | Value                                                             |
| --------- | ----------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#isMemberOf`                                |
| Domain(s) | [womo:Member](https://w3id.org/womo#Member) (c)<br />             |
| Range(s)  | [womo:Organization](https://w3id.org/womo#Organization) (c)<br /> |

[](isNaturalVentilationControlTypeOf)

### isNaturalVentilationControlTypeOf

| Property  | Value                                                                                               |
| --------- | --------------------------------------------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#isNaturalVentilationControlTypeOf`                                           |
| Domain(s) | [womo:NaturalVentilationControlType](https://w3id.org/womo#NaturalVentilationControlType) (c)<br /> |
| Range(s)  | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br />                                         |

[](isPartOf)

### isPartOf

| Property  | Value                                                             |
| --------- | ----------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#isPartOf`                                  |
| Domain(s) | [womo:Organization](https://w3id.org/womo#Organization) (c)<br /> |
| Range(s)  | [womo:Organization](https://w3id.org/womo#Organization) (c)<br /> |

[](isPerformedAt)

### isPerformedAt

| Property  | Value                                                       |
| --------- | ----------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#isPerformedAt`                       |
| Domain(s) | [womo:Activity](https://w3id.org/womo#Activity) (c)<br />   |
| Range(s)  | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br /> |

[](isPerformedBy)

### isPerformedBy

| Property  | Value                                                     |
| --------- | --------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#isPerformedBy`                     |
| Domain(s) | [womo:Activity](https://w3id.org/womo#Activity) (c)<br /> |
| Range(s)  | [womo:Worker](https://w3id.org/womo#Worker) (c)<br />     |

[](isPreferenceFor)

### isPreferenceFor

| Property  | Value                                                         |
| --------- | ------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#isPreferenceFor`                       |
| Domain(s) | [womo:Preference](https://w3id.org/womo#Preference) (c)<br /> |
| Range(s)  | [ssn:Property](http://www.w3.org/ns/ssn/Property) (c)<br />   |

[](isPreferredAs)

### isPreferredAs

| Property  | Value                                                         |
| --------- | ------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#isPreferredAs`                         |
| Domain(s) | [ssn:Property](http://www.w3.org/ns/ssn/Property) (c)<br />   |
| Range(s)  | [womo:Preference](https://w3id.org/womo#Preference) (c)<br /> |

[](isProvidedAt)

### isProvidedAt

| Property  | Value                                                       |
| --------- | ----------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#isProvidedAt`                        |
| Domain(s) | [womo:Feedback](https://w3id.org/womo#Feedback) (c)<br />   |
| Range(s)  | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br /> |

[](isProvidedBy)

### isProvidedBy

| Property  | Value                                                     |
| --------- | --------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#isProvidedBy`                      |
| Domain(s) | [womo:Feedback](https://w3id.org/womo#Feedback) (c)<br /> |
| Range(s)  | [womo:Worker](https://w3id.org/womo#Worker) (c)<br />     |

[](isRatingScaleOf)

### isRatingScaleOf

| Property  | Value                                                                                                                    |
| --------- | ------------------------------------------------------------------------------------------------------------------------ |
| IRI       | `https://w3id.org/womo#isRatingScaleOf`                                                                                  |
| Domain(s) | [womo:RatingScale](https://w3id.org/womo#RatingScale) (c)<br />                                                          |
| Range(s)  | [womo:Condition](https://w3id.org/womo#Condition) (c)<br />[womo:Preference](https://w3id.org/womo#Preference) (c)<br /> |

[](isRelatedTo)

### isRelatedTo

| Property  | Value                                                       |
| --------- | ----------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#isRelatedTo`                         |
| Domain(s) | [ssn:Property](http://www.w3.org/ns/ssn/Property) (c)<br /> |
| Range(s)  | [ssn:Property](http://www.w3.org/ns/ssn/Property) (c)<br /> |

[](isReportedBy)

### isReportedBy

| Property  | Value                                                                                                                        |
| --------- | ---------------------------------------------------------------------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#isReportedBy`                                                                                         |
| Domain(s) | ([womo:Activity](https://w3id.org/womo#Activity) (c) or [womo:WorkerFeature](https://w3id.org/womo#WorkerFeature) (c))<br /> |
| Range(s)  | [womo:Feedback](https://w3id.org/womo#Feedback) (c)<br />                                                                    |

[](isSocialInteractionOf)

### isSocialInteractionOf

| Property  | Value                                                                       |
| --------- | --------------------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#isSocialInteractionOf`                               |
| Domain(s) | [womo:SocialInteraction](https://w3id.org/womo#SocialInteraction) (c)<br /> |
| Range(s)  | [womo:Activity](https://w3id.org/womo#Activity) (c)<br />                   |

[](isVentilationTypeOf)

### isVentilationTypeOf

| Property  | Value                                                                   |
| --------- | ----------------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#isVentilationTypeOf`                             |
| Domain(s) | [womo:VentilationType](https://w3id.org/womo#VentilationType) (c)<br /> |
| Range(s)  | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br />             |

[](isWorkerFeatureOf)

### isWorkerFeatureOf

| Property  | Value                                                               |
| --------- | ------------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#isWorkerFeatureOf`                           |
| Domain(s) | [womo:WorkerFeature](https://w3id.org/womo#WorkerFeature) (c)<br /> |
| Range(s)  | [womo:Worker](https://w3id.org/womo#Worker) (c)<br />               |

[](isWorkspaceOf)

### isWorkspaceOf

| Property  | Value                                                             |
| --------- | ----------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#isWorkspaceOf`                             |
| Domain(s) | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br />       |
| Range(s)  | [womo:Organization](https://w3id.org/womo#Organization) (c)<br /> |

[](isWorkspaceTypeOf)

### isWorkspaceTypeOf

| Property  | Value                                                               |
| --------- | ------------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#isWorkspaceTypeOf`                           |
| Domain(s) | [womo:WorkspaceType](https://w3id.org/womo#WorkspaceType) (c)<br /> |
| Range(s)  | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br />         |

[](ownsWorkspace)

### ownsWorkspace

| Property  | Value                                                             |
| --------- | ----------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#ownsWorkspace`                             |
| Domain(s) | [womo:Organization](https://w3id.org/womo#Organization) (c)<br /> |
| Range(s)  | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br />       |

[](performs)

### performs

| Property  | Value                                                     |
| --------- | --------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#performs`                          |
| Domain(s) | [womo:Worker](https://w3id.org/womo#Worker) (c)<br />     |
| Range(s)  | [womo:Activity](https://w3id.org/womo#Activity) (c)<br /> |

[](provides)

### provides

| Property  | Value                                                     |
| --------- | --------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#provides`                          |
| Domain(s) | [womo:Worker](https://w3id.org/womo#Worker) (c)<br />     |
| Range(s)  | [womo:Feedback](https://w3id.org/womo#Feedback) (c)<br /> |

[](reports)

### reports

| Property  | Value                                                                                                                        |
| --------- | ---------------------------------------------------------------------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#reports`                                                                                              |
| Domain(s) | [womo:Feedback](https://w3id.org/womo#Feedback) (c)<br />                                                                    |
| Range(s)  | [womo:Activity](https://w3id.org/womo#Activity) (c)<br />[womo:WorkerFeature](https://w3id.org/womo#WorkerFeature) (c)<br /> |

[](supportsActivityType)

### supportsActivityType

| Property  | Value                                                             |
| --------- | ----------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#supportsActivityType`                      |
| Domain(s) | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br />       |
| Range(s)  | [womo:ActivityType](https://w3id.org/womo#ActivityType) (c)<br /> |

## Datatype Properties

[feedbackRequestTime](#feedbackRequestTime),
[feedbackStartTime](#feedbackStartTime),
[feedbackTime](#feedbackTime),
[fromIFCDatatypeProperties](#fromIFCDatatypeProperties),
[organizationLogo](#organizationLogo),
[organizationName](#organizationName),
[rating](#rating),
[ratingScaleName](#ratingScaleName),
[ratingScaleOptions](#ratingScaleOptions),
[ratingScalePrompt](#ratingScalePrompt),
[responseDuration](#responseDuration),
[responseRatio](#responseRatio),
[value](#value),
[workspaceAreaPerOccupant](#workspaceAreaPerOccupant),
[workspaceHeight](#workspaceHeight),
[workspaceIsShared](#workspaceIsShared),
[workspaceLocalID](#workspaceLocalID),
[workspaceNetFloorArea](#workspaceNetFloorArea),
[workspaceNetVolume](#workspaceNetVolume),
[workspaceOccupancyNumber](#workspaceOccupancyNumber),
[workspacePubliclyAccessible](#workspacePubliclyAccessible),
[workspaceVolumePerOccupant](#workspaceVolumePerOccupant),
[](feedbackRequestTime)

### feedbackRequestTime

| Property    | Value                                                               |
| ----------- | ------------------------------------------------------------------- |
| IRI         | `https://w3id.org/womo#feedbackRequestTime`                         |
| Description | Time of feedback request.                                           |
| Domain(s)   | [womo:Feedback](https://w3id.org/womo#Feedback) (c)<br />           |
| Range(s)    | [xsd:dateTime](http://www.w3.org/2001/XMLSchema#dateTime) (c)<br /> |

[](feedbackStartTime)

### feedbackStartTime

| Property    | Value                                                               |
| ----------- | ------------------------------------------------------------------- |
| IRI         | `https://w3id.org/womo#feedbackStartTime`                           |
| Description | Time of feedback response start.                                    |
| Domain(s)   | [womo:Feedback](https://w3id.org/womo#Feedback) (c)<br />           |
| Range(s)    | [xsd:dateTime](http://www.w3.org/2001/XMLSchema#dateTime) (c)<br /> |

[](feedbackTime)

### feedbackTime

| Property    | Value                                                               |
| ----------- | ------------------------------------------------------------------- |
| IRI         | `https://w3id.org/womo#feedbackTime`                                |
| Description | Time of feedback response conclusion.                               |
| Domain(s)   | [womo:Feedback](https://w3id.org/womo#Feedback) (c)<br />           |
| Range(s)    | [xsd:dateTime](http://www.w3.org/2001/XMLSchema#dateTime) (c)<br /> |

[](fromIFCDatatypeProperties)

### fromIFCDatatypeProperties

| Property | Value                                             |
| -------- | ------------------------------------------------- |
| IRI      | `https://w3id.org/womo#fromIFCDatatypeProperties` |

[](organizationLogo)

### organizationLogo

| Property  | Value                                                             |
| --------- | ----------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#organizationLogo`                          |
| Domain(s) | [womo:Organization](https://w3id.org/womo#Organization) (c)<br /> |
| Range(s)  | [xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />   |

[](organizationName)

### organizationName

| Property  | Value                                                             |
| --------- | ----------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#organizationName`                          |
| Domain(s) | [womo:Organization](https://w3id.org/womo#Organization) (c)<br /> |
| Range(s)  | [xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />   |

[](rating)

### rating

| Property  | Value                                                                                                                    |
| --------- | ------------------------------------------------------------------------------------------------------------------------ |
| IRI       | `https://w3id.org/womo#rating`                                                                                           |
| Domain(s) | ([womo:Condition](https://w3id.org/womo#Condition) (c) or [womo:Preference](https://w3id.org/womo#Preference) (c))<br /> |
| Range(s)  | [xsd:integer](http://www.w3.org/2001/XMLSchema#integer) (c)<br />                                                        |

[](ratingScaleName)

### ratingScaleName

| Property  | Value                                                           |
| --------- | --------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#ratingScaleName`                         |
| Domain(s) | [womo:RatingScale](https://w3id.org/womo#RatingScale) (c)<br /> |
| Range(s)  | [xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br /> |

[](ratingScaleOptions)

### ratingScaleOptions

| Property  | Value                                                           |
| --------- | --------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#ratingScaleOptions`                      |
| Domain(s) | [womo:RatingScale](https://w3id.org/womo#RatingScale) (c)<br /> |
| Range(s)  | [xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br /> |

[](ratingScalePrompt)

### ratingScalePrompt

| Property  | Value                                                           |
| --------- | --------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#ratingScalePrompt`                       |
| Domain(s) | [womo:RatingScale](https://w3id.org/womo#RatingScale) (c)<br /> |
| Range(s)  | [xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br /> |

[](responseDuration)

### responseDuration

| Property    | Value                                                              |
| ----------- | ------------------------------------------------------------------ |
| IRI         | `https://w3id.org/womo#responseDuration`                           |
| Description | Elapsed time between feedback response start and conclusion (sec). |
| Domain(s)   | [womo:Feedback](https://w3id.org/womo#Feedback) (c)<br />          |
| Range(s)    | [xsd:integer](http://www.w3.org/2001/XMLSchema#integer) (c)<br />  |

[](responseRatio)

### responseRatio

| Property    | Value                                                             |
| ----------- | ----------------------------------------------------------------- |
| IRI         | `https://w3id.org/womo#responseRatio`                             |
| Description | Ratio of answered questions (%).                                  |
| Domain(s)   | [womo:Feedback](https://w3id.org/womo#Feedback) (c)<br />         |
| Range(s)    | [xsd:integer](http://www.w3.org/2001/XMLSchema#integer) (c)<br /> |

[](value)

### value

| Property  | Value                                                                   |
| --------- | ----------------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#value`                                           |
| Domain(s) | [womo:HealthIndicator](https://w3id.org/womo#HealthIndicator) (c)<br /> |
| Range(s)  | [xsd:float](http://www.w3.org/2001/XMLSchema#float) (c)<br />           |

[](workspaceAreaPerOccupant)

### workspaceAreaPerOccupant

| Property         | Value                                                                                        |
| ---------------- | -------------------------------------------------------------------------------------------- |
| IRI              | `https://w3id.org/womo#workspaceAreaPerOccupant`                                             |
| Super-properties | [womo:fromIFCDatatypeProperties](https://w3id.org/womo#fromIFCDatatypeProperties) (dp)<br /> |
| Domain(s)        | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br />                                  |
| Range(s)         | [xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />                            |

[](workspaceHeight)

### workspaceHeight

| Property         | Value                                                                                        |
| ---------------- | -------------------------------------------------------------------------------------------- |
| IRI              | `https://w3id.org/womo#workspaceHeight`                                                      |
| Super-properties | [womo:fromIFCDatatypeProperties](https://w3id.org/womo#fromIFCDatatypeProperties) (dp)<br /> |
| Domain(s)        | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br />                                  |
| Range(s)         | [xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />                            |

[](workspaceIsShared)

### workspaceIsShared

| Property  | Value                                                             |
| --------- | ----------------------------------------------------------------- |
| IRI       | `https://w3id.org/womo#workspaceIsShared`                         |
| Domain(s) | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br />       |
| Range(s)  | [xsd:boolean](http://www.w3.org/2001/XMLSchema#boolean) (c)<br /> |

[](workspaceLocalID)

### workspaceLocalID

| Property         | Value                                                                                        |
| ---------------- | -------------------------------------------------------------------------------------------- |
| IRI              | `https://w3id.org/womo#workspaceLocalID`                                                     |
| Super-properties | [womo:fromIFCDatatypeProperties](https://w3id.org/womo#fromIFCDatatypeProperties) (dp)<br /> |
| Domain(s)        | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br />                                  |
| Range(s)         | [xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />                              |

[](workspaceNetFloorArea)

### workspaceNetFloorArea

| Property         | Value                                                                                        |
| ---------------- | -------------------------------------------------------------------------------------------- |
| IRI              | `https://w3id.org/womo#workspaceNetFloorArea`                                                |
| Super-properties | [womo:fromIFCDatatypeProperties](https://w3id.org/womo#fromIFCDatatypeProperties) (dp)<br /> |
| Domain(s)        | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br />                                  |
| Range(s)         | [xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />                            |

[](workspaceNetVolume)

### workspaceNetVolume

| Property         | Value                                                                                        |
| ---------------- | -------------------------------------------------------------------------------------------- |
| IRI              | `https://w3id.org/womo#workspaceNetVolume`                                                   |
| Super-properties | [womo:fromIFCDatatypeProperties](https://w3id.org/womo#fromIFCDatatypeProperties) (dp)<br /> |
| Domain(s)        | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br />                                  |
| Range(s)         | [xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />                            |

[](workspaceOccupancyNumber)

### workspaceOccupancyNumber

| Property         | Value                                                                                        |
| ---------------- | -------------------------------------------------------------------------------------------- |
| IRI              | `https://w3id.org/womo#workspaceOccupancyNumber`                                             |
| Super-properties | [womo:fromIFCDatatypeProperties](https://w3id.org/womo#fromIFCDatatypeProperties) (dp)<br /> |
| Domain(s)        | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br />                                  |
| Range(s)         | [xsd:integer](http://www.w3.org/2001/XMLSchema#integer) (c)<br />                            |

[](workspacePubliclyAccessible)

### workspacePubliclyAccessible

| Property         | Value                                                                                        |
| ---------------- | -------------------------------------------------------------------------------------------- |
| IRI              | `https://w3id.org/womo#workspacePubliclyAccessible`                                          |
| Super-properties | [womo:fromIFCDatatypeProperties](https://w3id.org/womo#fromIFCDatatypeProperties) (dp)<br /> |
| Domain(s)        | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br />                                  |
| Range(s)         | [xsd:boolean](http://www.w3.org/2001/XMLSchema#boolean) (c)<br />                            |

[](workspaceVolumePerOccupant)

### workspaceVolumePerOccupant

| Property         | Value                                                                                        |
| ---------------- | -------------------------------------------------------------------------------------------- |
| IRI              | `https://w3id.org/womo#workspaceVolumePerOccupant`                                           |
| Super-properties | [womo:fromIFCDatatypeProperties](https://w3id.org/womo#fromIFCDatatypeProperties) (dp)<br /> |
| Domain(s)        | [womo:Workspace](https://w3id.org/womo#Workspace) (c)<br />                                  |
| Range(s)         | [xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />                            |

## Named Individuals

[AcousticQuality](#AcousticQuality),
[AirQuality](#AirQuality),
[AirTemperature](#AirTemperature),
[AutomaticMVControlOnly](#AutomaticMVControlOnly),
[AutomaticNVControlOnly](#AutomaticNVControlOnly),
[Away](#Away),
[Break](#Break),
[BreakCoffee](#BreakCoffee),
[BreakMeal](#BreakMeal),
[BreakUnspecified](#BreakUnspecified),
[Busy](#Busy),
[CO2Concentration](#CO2Concentration),
[Concentration](#Concentration),
[Concentration3PointsScale](#Concentration3PointsScale),
[ConferenceRoom](#ConferenceRoom),
[Cubicle](#Cubicle),
[DailyStepCount](#DailyStepCount),
[Direct](#Direct),
[EventFeedback](#EventFeedback),
[Group](#Group),
[HeartRate](#HeartRate),
[HomeOffice](#HomeOffice),
[Illuminance](#Illuminance),
[IndirectVentilationOnly](#IndirectVentilationOnly),
[Inferred_MeanVal_Hour](#Inferred_MeanVal_Hour),
[Inferred_SingleVal](#Inferred_SingleVal),
[ManualMVControlOnly](#ManualMVControlOnly),
[ManualNVControlOnly](#ManualNVControlOnly),
[MechanicalVentilationOnly](#MechanicalVentilationOnly),
[MixedMVControl](#MixedMVControl),
[MixedNVControl](#MixedNVControl),
[MixedVentilation](#MixedVentilation),
[NaturalVentilationOnly](#NaturalVentilationOnly),
[NoiseLevel](#NoiseLevel),
[Observed_SingleVal](#Observed_SingleVal),
[OccupancyCount](#OccupancyCount),
[OccupancyRatio](#OccupancyRatio),
[OpenOffice](#OpenOffice),
[Pair](#Pair),
[Postponed](#Postponed),
[PrivateOffice](#PrivateOffice),
[Productivity](#Productivity),
[Productivity3PointsScale](#Productivity3PointsScale),
[RandomFeedback](#RandomFeedback),
[RelativeHumidity](#RelativeHumidity),
[ScheduledFeedback](#ScheduledFeedback),
[SharedOffice](#SharedOffice),
[SmallGroup](#SmallGroup),
[Solo](#Solo),
[TeamRoom](#TeamRoom),
[ThermalQuality](#ThermalQuality),
[ThermalQuality3PointsScale](#ThermalQuality3PointsScale),
[Timeout](#Timeout),
[Unspecified](#Unspecified),
[VisualQuality](#VisualQuality),
[VoluntaryFeedback](#VoluntaryFeedback),
[Work](#Work),
[WorkCall](#WorkCall),
[WorkGroup](#WorkGroup),
[WorkSolo](#WorkSolo),
[WorkUnspecified](#WorkUnspecified),

### AcousticQuality <sup>c</sup>

| Property | Value                                   |
| -------- | --------------------------------------- |
| IRI      | `https://w3id.org/womo#AcousticQuality` |

- **Contributor(s)**
  - [ssn:Property](http://www.w3.org/ns/ssn/Property)

### AirQuality <sup>c</sup>

| Property | Value                              |
| -------- | ---------------------------------- |
| IRI      | `https://w3id.org/womo#AirQuality` |

- **Contributor(s)**
  - [ssn:Property](http://www.w3.org/ns/ssn/Property)

### AirTemperature <sup>c</sup>

| Property | Value                                  |
| -------- | -------------------------------------- |
| IRI      | `https://w3id.org/womo#AirTemperature` |

- **Contributor(s)**
  - [sosa:ObservableProperty](http://www.w3.org/ns/sosa/ObservableProperty)

### AutomaticMVControlOnly <sup>c</sup>

| Property | Value                                          |
| -------- | ---------------------------------------------- |
| IRI      | `https://w3id.org/womo#AutomaticMVControlOnly` |

- **Contributor(s)**
  - [womo:MechanicalVentilationControlType](https://w3id.org/womo#MechanicalVentilationControlType)

### AutomaticNVControlOnly <sup>c</sup>

| Property | Value                                          |
| -------- | ---------------------------------------------- |
| IRI      | `https://w3id.org/womo#AutomaticNVControlOnly` |

- **Contributor(s)**
  - [womo:NaturalVentilationControlType](https://w3id.org/womo#NaturalVentilationControlType)

### Away <sup>c</sup>

| Property | Value                        |
| -------- | ---------------------------- |
| IRI      | `https://w3id.org/womo#Away` |

- **Contributor(s)**
  - [womo:NotRespondedFeedback](https://w3id.org/womo#NotRespondedFeedback)
    Description | Feedback request declined because the worker is not at the workplace.

### Break <sup>c</sup>

| Property | Value                         |
| -------- | ----------------------------- |
| IRI      | `https://w3id.org/womo#Break` |

- **Contributor(s)**
  - [womo:ActivityCategory](https://w3id.org/womo#ActivityCategory)
    Description | Activity that is a break from the worker's job.

### BreakCoffee <sup>c</sup>

| Property | Value                               |
| -------- | ----------------------------------- |
| IRI      | `https://w3id.org/womo#BreakCoffee` |

- **Contributor(s)**
  - [womo:ActivityType](https://w3id.org/womo#ActivityType)
    Description | Coffee break, usually short.

### BreakMeal <sup>c</sup>

| Property | Value                             |
| -------- | --------------------------------- |
| IRI      | `https://w3id.org/womo#BreakMeal` |

- **Contributor(s)**
  - [womo:ActivityType](https://w3id.org/womo#ActivityType)
    Description | Break involving a meal. (e.g. lunch)

### BreakUnspecified <sup>c</sup>

| Property | Value                                    |
| -------- | ---------------------------------------- |
| IRI      | `https://w3id.org/womo#BreakUnspecified` |

- **Contributor(s)**
  - [womo:ActivityType](https://w3id.org/womo#ActivityType)
    Description | Unspecified break.

### Busy <sup>c</sup>

| Property | Value                        |
| -------- | ---------------------------- |
| IRI      | `https://w3id.org/womo#Busy` |

- **Contributor(s)**
  - [womo:NotRespondedFeedback](https://w3id.org/womo#NotRespondedFeedback)
    Description | Feedback request declined because the worker is too busy.

### CO2Concentration <sup>c</sup>

| Property | Value                                    |
| -------- | ---------------------------------------- |
| IRI      | `https://w3id.org/womo#CO2Concentration` |

- **Contributor(s)**
  - [sosa:ObservableProperty](http://www.w3.org/ns/sosa/ObservableProperty)

### Concentration <sup>c</sup>

| Property | Value                                 |
| -------- | ------------------------------------- |
| IRI      | `https://w3id.org/womo#Concentration` |

- **Contributor(s)**
  - [womo:ConditionType](https://w3id.org/womo#ConditionType)

### Concentration3PointsScale <sup>c</sup>

| Property | Value                                             |
| -------- | ------------------------------------------------- |
| IRI      | `https://w3id.org/womo#Concentration3PointsScale` |

- **Contributor(s)**
  - [womo:RatingScale](https://w3id.org/womo#RatingScale)

### ConferenceRoom <sup>c</sup>

| Property | Value                                  |
| -------- | -------------------------------------- |
| IRI      | `https://w3id.org/womo#ConferenceRoom` |

- **Contributor(s)**
  - [womo:Room](https://w3id.org/womo#Room)

### Cubicle <sup>c</sup>

| Property | Value                           |
| -------- | ------------------------------- |
| IRI      | `https://w3id.org/womo#Cubicle` |

- **Contributor(s)**
  - [womo:Office](https://w3id.org/womo#Office)

### DailyStepCount <sup>c</sup>

| Property | Value                                  |
| -------- | -------------------------------------- |
| IRI      | `https://w3id.org/womo#DailyStepCount` |

- **Contributor(s)**
  - [womo:HealthIndicatorType](https://w3id.org/womo#HealthIndicatorType)
    Description | Daily step count measured in (step).

### Direct <sup>c</sup>

| Property | Value                          |
| -------- | ------------------------------ |
| IRI      | `https://w3id.org/womo#Direct` |

- **Contributor(s)**
  - [womo:RespondedFeedback](https://w3id.org/womo#RespondedFeedback)
    Description | Feedback request responded directly.

### EventFeedback <sup>c</sup>

| Property | Value                                 |
| -------- | ------------------------------------- |
| IRI      | `https://w3id.org/womo#EventFeedback` |

- **Contributor(s)**
  - [womo:FeedbackGenerationType](https://w3id.org/womo#FeedbackGenerationType)
    Description | Indicates a feedback request triggered by an event.

### Group <sup>c</sup>

| Property | Value                         |
| -------- | ----------------------------- |
| IRI      | `https://w3id.org/womo#Group` |

- **Contributor(s)**
  - [womo:SocialInteraction](https://w3id.org/womo#SocialInteraction)
    Description | The worker is performing the activity in a larger group. Total of 5 or more workers.

### HeartRate <sup>c</sup>

| Property | Value                             |
| -------- | --------------------------------- |
| IRI      | `https://w3id.org/womo#HeartRate` |

- **Contributor(s)**
  - [womo:HealthIndicatorType](https://w3id.org/womo#HealthIndicatorType)
    Description | Heart rate measured in (bpm).

### HomeOffice <sup>c</sup>

| Property | Value                              |
| -------- | ---------------------------------- |
| IRI      | `https://w3id.org/womo#HomeOffice` |

- **Contributor(s)**
  - [womo:NotRespondedFeedback](https://w3id.org/womo#NotRespondedFeedback)
    Description | Feedback request declined because the worker is working from home.

### Illuminance <sup>c</sup>

| Property | Value                               |
| -------- | ----------------------------------- |
| IRI      | `https://w3id.org/womo#Illuminance` |

- **Contributor(s)**
  - [sosa:ObservableProperty](http://www.w3.org/ns/sosa/ObservableProperty)

### IndirectVentilationOnly <sup>c</sup>

| Property | Value                                           |
| -------- | ----------------------------------------------- |
| IRI      | `https://w3id.org/womo#IndirectVentilationOnly` |

- **Contributor(s)**
  - [womo:VentilationType](https://w3id.org/womo#VentilationType)

### Inferred_MeanVal_Hour <sup>c</sup>

| Property | Value                                         |
| -------- | --------------------------------------------- |
| IRI      | `https://w3id.org/womo#Inferred_MeanVal_Hour` |

- **Contributor(s)**
  - [sosa:Procedure](http://www.w3.org/ns/sosa/Procedure)

### Inferred_SingleVal <sup>c</sup>

| Property | Value                                      |
| -------- | ------------------------------------------ |
| IRI      | `https://w3id.org/womo#Inferred_SingleVal` |

- **Contributor(s)**
  - [sosa:Procedure](http://www.w3.org/ns/sosa/Procedure)

### ManualMVControlOnly <sup>c</sup>

| Property | Value                                       |
| -------- | ------------------------------------------- |
| IRI      | `https://w3id.org/womo#ManualMVControlOnly` |

- **Contributor(s)**
  - [womo:MechanicalVentilationControlType](https://w3id.org/womo#MechanicalVentilationControlType)

### ManualNVControlOnly <sup>c</sup>

| Property | Value                                       |
| -------- | ------------------------------------------- |
| IRI      | `https://w3id.org/womo#ManualNVControlOnly` |

- **Contributor(s)**
  - [womo:NaturalVentilationControlType](https://w3id.org/womo#NaturalVentilationControlType)

### MechanicalVentilationOnly <sup>c</sup>

| Property | Value                                             |
| -------- | ------------------------------------------------- |
| IRI      | `https://w3id.org/womo#MechanicalVentilationOnly` |

- **Contributor(s)**
  - [womo:VentilationType](https://w3id.org/womo#VentilationType)

### MixedMVControl <sup>c</sup>

| Property | Value                                  |
| -------- | -------------------------------------- |
| IRI      | `https://w3id.org/womo#MixedMVControl` |

- **Contributor(s)**
  - [womo:MechanicalVentilationControlType](https://w3id.org/womo#MechanicalVentilationControlType)

### MixedNVControl <sup>c</sup>

| Property | Value                                  |
| -------- | -------------------------------------- |
| IRI      | `https://w3id.org/womo#MixedNVControl` |

- **Contributor(s)**
  - [womo:NaturalVentilationControlType](https://w3id.org/womo#NaturalVentilationControlType)

### MixedVentilation <sup>c</sup>

| Property | Value                                    |
| -------- | ---------------------------------------- |
| IRI      | `https://w3id.org/womo#MixedVentilation` |

- **Contributor(s)**
  - [womo:VentilationType](https://w3id.org/womo#VentilationType)

### NaturalVentilationOnly <sup>c</sup>

| Property | Value                                          |
| -------- | ---------------------------------------------- |
| IRI      | `https://w3id.org/womo#NaturalVentilationOnly` |

- **Contributor(s)**
  - [womo:VentilationType](https://w3id.org/womo#VentilationType)

### NoiseLevel <sup>c</sup>

| Property | Value                              |
| -------- | ---------------------------------- |
| IRI      | `https://w3id.org/womo#NoiseLevel` |

- **Contributor(s)**
  - [sosa:ObservableProperty](http://www.w3.org/ns/sosa/ObservableProperty)

### Observed_SingleVal <sup>c</sup>

| Property | Value                                      |
| -------- | ------------------------------------------ |
| IRI      | `https://w3id.org/womo#Observed_SingleVal` |

- **Contributor(s)**
  - [sosa:Procedure](http://www.w3.org/ns/sosa/Procedure)

### OccupancyCount <sup>c</sup>

| Property | Value                                  |
| -------- | -------------------------------------- |
| IRI      | `https://w3id.org/womo#OccupancyCount` |

- **Contributor(s)**
  - [sosa:ObservableProperty](http://www.w3.org/ns/sosa/ObservableProperty)

### OccupancyRatio <sup>c</sup>

| Property | Value                                  |
| -------- | -------------------------------------- |
| IRI      | `https://w3id.org/womo#OccupancyRatio` |

- **Contributor(s)**
  - [sosa:ObservableProperty](http://www.w3.org/ns/sosa/ObservableProperty)

### OpenOffice <sup>c</sup>

| Property | Value                              |
| -------- | ---------------------------------- |
| IRI      | `https://w3id.org/womo#OpenOffice` |

- **Contributor(s)**
  - [womo:Office](https://w3id.org/womo#Office)

### Pair <sup>c</sup>

| Property | Value                        |
| -------- | ---------------------------- |
| IRI      | `https://w3id.org/womo#Pair` |

- **Contributor(s)**
  - [womo:SocialInteraction](https://w3id.org/womo#SocialInteraction)
    Description | The worker is doing the activity together with another colleaugue.

### Postponed <sup>c</sup>

| Property | Value                             |
| -------- | --------------------------------- |
| IRI      | `https://w3id.org/womo#Postponed` |

- **Contributor(s)**
  - [womo:RespondedFeedback](https://w3id.org/womo#RespondedFeedback)
    Description | Feedback request responded after being postponed.

### PrivateOffice <sup>c</sup>

| Property | Value                                 |
| -------- | ------------------------------------- |
| IRI      | `https://w3id.org/womo#PrivateOffice` |

- **Contributor(s)**
  - [womo:EnclosedOffice](https://w3id.org/womo#EnclosedOffice)

### Productivity <sup>c</sup>

| Property | Value                                |
| -------- | ------------------------------------ |
| IRI      | `https://w3id.org/womo#Productivity` |

- **Contributor(s)**
  - [womo:ConditionType](https://w3id.org/womo#ConditionType)

### Productivity3PointsScale <sup>c</sup>

| Property | Value                                            |
| -------- | ------------------------------------------------ |
| IRI      | `https://w3id.org/womo#Productivity3PointsScale` |

- **Contributor(s)**
  - [womo:RatingScale](https://w3id.org/womo#RatingScale)

### RandomFeedback <sup>c</sup>

| Property | Value                                  |
| -------- | -------------------------------------- |
| IRI      | `https://w3id.org/womo#RandomFeedback` |

- **Contributor(s)**
  - [womo:FeedbackGenerationType](https://w3id.org/womo#FeedbackGenerationType)
    Description | Indicates a feedback request generated at a random time within a daily time frame (e.g. 9:00-11:00 AM).

### RelativeHumidity <sup>c</sup>

| Property | Value                                    |
| -------- | ---------------------------------------- |
| IRI      | `https://w3id.org/womo#RelativeHumidity` |

- **Contributor(s)**
  - [sosa:ObservableProperty](http://www.w3.org/ns/sosa/ObservableProperty)

### ScheduledFeedback <sup>c</sup>

| Property | Value                                     |
| -------- | ----------------------------------------- |
| IRI      | `https://w3id.org/womo#ScheduledFeedback` |

- **Contributor(s)**
  - [womo:FeedbackGenerationType](https://w3id.org/womo#FeedbackGenerationType)
    Description | Indicates a feedback request generated at a scheduled time (e.g. 13:00).

### SharedOffice <sup>c</sup>

| Property | Value                                |
| -------- | ------------------------------------ |
| IRI      | `https://w3id.org/womo#SharedOffice` |

- **Contributor(s)**
  - [womo:EnclosedOffice](https://w3id.org/womo#EnclosedOffice)

### SmallGroup <sup>c</sup>

| Property | Value                              |
| -------- | ---------------------------------- |
| IRI      | `https://w3id.org/womo#SmallGroup` |

- **Contributor(s)**
  - [womo:SocialInteraction](https://w3id.org/womo#SocialInteraction)
    Description | The worker is performing the activity in a small group. Total of 3 or 4 workers.

### Solo <sup>c</sup>

| Property | Value                        |
| -------- | ---------------------------- |
| IRI      | `https://w3id.org/womo#Solo` |

- **Contributor(s)**
  - [womo:SocialInteraction](https://w3id.org/womo#SocialInteraction)
    Description | The worker is doing the activity on his own.

### TeamRoom <sup>c</sup>

| Property | Value                            |
| -------- | -------------------------------- |
| IRI      | `https://w3id.org/womo#TeamRoom` |

- **Contributor(s)**
  - [womo:EnclosedOffice](https://w3id.org/womo#EnclosedOffice)

### ThermalQuality <sup>c</sup>

| Property | Value                                  |
| -------- | -------------------------------------- |
| IRI      | `https://w3id.org/womo#ThermalQuality` |

- **Contributor(s)**
  - [ssn:Property](http://www.w3.org/ns/ssn/Property)

### ThermalQuality3PointsScale <sup>c</sup>

| Property | Value                                              |
| -------- | -------------------------------------------------- |
| IRI      | `https://w3id.org/womo#ThermalQuality3PointsScale` |

- **Contributor(s)**
  - [womo:RatingScale](https://w3id.org/womo#RatingScale)

### Timeout <sup>c</sup>

| Property | Value                           |
| -------- | ------------------------------- |
| IRI      | `https://w3id.org/womo#Timeout` |

- **Contributor(s)**
  - [womo:NotRespondedFeedback](https://w3id.org/womo#NotRespondedFeedback)
    Description | Feedback request canceled after timeout.

### Unspecified <sup>c</sup>

| Property | Value                               |
| -------- | ----------------------------------- |
| IRI      | `https://w3id.org/womo#Unspecified` |

- **Contributor(s)**
  - [womo:NotRespondedFeedback](https://w3id.org/womo#NotRespondedFeedback)
    Description | Feedback request declined for unspecified reasons.

### VisualQuality <sup>c</sup>

| Property | Value                                 |
| -------- | ------------------------------------- |
| IRI      | `https://w3id.org/womo#VisualQuality` |

- **Contributor(s)**
  - [ssn:Property](http://www.w3.org/ns/ssn/Property)

### VoluntaryFeedback <sup>c</sup>

| Property | Value                                     |
| -------- | ----------------------------------------- |
| IRI      | `https://w3id.org/womo#VoluntaryFeedback` |

- **Contributor(s)**
  - [womo:FeedbackGenerationType](https://w3id.org/womo#FeedbackGenerationType)
    Description | Indicates a feedback provided voluntarily by the worker/occupant at a given time.

### Work <sup>c</sup>

| Property | Value                        |
| -------- | ---------------------------- |
| IRI      | `https://w3id.org/womo#Work` |

- **Contributor(s)**
  - [womo:ActivityCategory](https://w3id.org/womo#ActivityCategory)
    Description | Activity that is part of the the worker's job.

### WorkCall <sup>c</sup>

| Property | Value                            |
| -------- | -------------------------------- |
| IRI      | `https://w3id.org/womo#WorkCall` |

- **Contributor(s)**
  - [womo:ActivityType](https://w3id.org/womo#ActivityType)
    Description | Work call or videocall.

### WorkGroup <sup>c</sup>

| Property | Value                             |
| -------- | --------------------------------- |
| IRI      | `https://w3id.org/womo#WorkGroup` |

- **Contributor(s)**
  - [womo:ActivityType](https://w3id.org/womo#ActivityType)
    Description | Work activity performed by the worker together with one or more colleagues.

### WorkSolo <sup>c</sup>

| Property | Value                            |
| -------- | -------------------------------- |
| IRI      | `https://w3id.org/womo#WorkSolo` |

- **Contributor(s)**
  - [womo:ActivityType](https://w3id.org/womo#ActivityType)
    Description | Work activity performed by the worker on his own.

### WorkUnspecified <sup>c</sup>

| Property | Value                                   |
| -------- | --------------------------------------- |
| IRI      | `https://w3id.org/womo#WorkUnspecified` |

- **Contributor(s)**
  - [womo:ActivityType](https://w3id.org/womo#ActivityType)
    Description | Unspecified work activity.

## Namespaces

- **dc**
  - `http://purl.org/dc/terms/`
- **ifcOWL**
  - `https://standards.buildingsmart.org/IFC/DEV/IFC4/ADD2_TC1/OWL#`
- **owl**
  - `http://www.w3.org/2002/07/owl#`
- **prov**
  - `http://www.w3.org/ns/prov#`
- **rdf**
  - `http://www.w3.org/1999/02/22-rdf-syntax-ns#`
- **rdfs**
  - `http://www.w3.org/2000/01/rdf-schema#`
- **sdo**
  - `https://schema.org/`
- **skos**
  - `http://www.w3.org/2004/02/skos/core#`
- **sosa**
  - `http://www.w3.org/ns/sosa/`
- **ssn**
  - `http://www.w3.org/ns/ssn/`
- **vann**
  - `http://purl.org/vocab/vann/`
- **womo**
  - `https://w3id.org/womo#`
- **xml**
  - `http://www.w3.org/XML/1998/namespace`
- **xsd**
  - `http://www.w3.org/2001/XMLSchema#`

## Legend

- Classes: c
- Object Properties: op
- Functional Properties: fp
- Data Properties: dp
- Annotation Properties: dp
- Properties: p
- Named Individuals: ni
