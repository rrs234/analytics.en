---
description: Use quick segments in Analysis Workspace.
title: Quick segments
feature: Workspace Basics
role: User, Admin
---

# Quick segments

You can create quick segments within a project to bypass the complexity of the full [segment builder](/help/components/segmentation/segmentation-workflow/seg-build.md). Quick segments

* Apply only to projects in which they were created (you can change this).
* Allow for up to 3 rules.
* Do not accommodate nested containers, or sequential rules.
* Do work in projects with multiple report suites.

For a comparison of what quick segments can do vs. full-fledged component-list segments, go [here](/help/analyze/analysis-workspace/components/segments/t-freeform-project-segment.md). 

>[!IMPORTANT]
> Quick segments are currently in limited testing and will be generally available on October 21, 2021.

## Prerequisites

Anyone can create a [!UICONTROL Quick Segment]. However, you need the[!UICONTROL Segment Creation] permission in the [Adobe Admin Console](https://experienceleague.adobe.com/docs/analytics/admin/admin-console/permissions/summary-tables.html?lang=en#analytics-tools) to be able to save a quick segments or to open it in the [!UICONTROL Segment Builder].

## Create quick segments

In a Freeform table, click the filter+ icon in the panel header: 

![](assets/quick-seg1.png)

| Setting | Description |
| --- | --- |
| Name | The default name of a segment is a combination of the rule names in the segment. You can rename the segment. |
| Include/exclude | You can either include or exclude components in your segment definition, but not both. |
| Hit/Visit/Visitor container | Quick segments include one [segment container](https://experienceleague.adobe.com/docs/analytics/components/segmentation/seg-overview.html?lang=en#section_AF2A28BE92474DB386AE85743C71B2D6) only that lets you include a dimension/metric/date range in (or exclude it from) the segment. [!UICONTROL Visitor] contains overarching data specific for the visitor across visits and page views. A [!UICONTROL Visit] container lets you set rules to break down the visitor’s data based on visits, and a [!UICONTROL Hit] container lets you break down visitor information based on individual page views. The default container is [!UICONTROL Hit]. |
| Components (Dimension/metric/date range) | Define up to 3 rules by adding components dimensions and/or metrics and/or date ranges and their values. There are 3 ways to find the right component:<ul><li>Start typing and the [!UICONTROL Quick Segment] builder automatically finds the appropriate component.</li><li>Use the drop-down list to find the component.</li><li>Drag and drop components from the left rail.</li></ul>  |
| Operator | Use the drop-down menu to find standard operators and [!UICONTROL Distinct Count] operators. [Learn more](https://experienceleague.adobe.com/docs/analytics/components/segmentation/segment-reference/seg-operators.html?lang=en) |
| Plus (+) sign | Add another rule |
| AND/OR qualifiers | You can add "AND" or "OR" qualifiers to the rules, but you cannot mix "AND" and "OR" in a single segment definition. |
| Apply | Apply this segment to the panel. If the segment contains no data, you will be asked if you want to continue. |
| Open builder | Opens the Segment Builder. Once you save the segment in the Segment Builder, it is no longer considered a "Quick Segment". It becomes part of the component-list segment library. |
| Cancel | Cancel this quick segment - don't apply it. |
| Date range | The validator uses the panel date range for its data lookup. But any date range applied in a quick segment overrides the panel date range at the top of the panel.  |
| Preview (top right) | Lets you see whether you have a valid segment and how broad the segment is. Represents the breakdown of the data set you can expect to see when you apply this segment. you might get a notice that indicates that this segment has no data. You can proceed or change the segment definition. |

Here is an example of a segment that combines dimensions and metrics:

![](assets/quick-seg2.png)

The segment appears at the top. Notice its blue-striped sidebar, as opposed to the blue sidebar for component-level segments in the segment library on the left.

![](assets/quick-seg5.png)

## Edit quick segments

1. Hover over the quick segment and select the pencil icon.
1. Edit the segment definition and/or the segment name.
1. Click [!UICONTROL Apply].

## Save quick segments

>[!IMPORTANT]
>Once you save or apply the segment, you can no longer edit it in the Quick Segment Builder, only in the regular Segment Builder.

1. Once you have applied the quick segment, hover over it and select the info ("i") icon.

   ![](assets/quick-seg6.png)

1. Click **[!UICONTROL Make available to all projects and add to your component list]**.
1. (Optional) Rename the segment.
1. Click **[!UICONTROL Save]**.

Notice how the segment's side bar changes from striped blue to blue. It now appears in your component list in the left rail.

## What are project-only segments?

Project-only segments are either quick segments or ad-hoc Workspace project segments. When editing/opening them in the [!UICONTROL Segment Builder], the project-only box will show up. If you APPLY a quick segment in the builder but don’t check the make available box, then it is still a project-only segment but it can no longer be opened in the [!UICONTROL Quick Segment Builder]. If you check the box and click **[!UICONTROL SAVE]**, it is now a component-list segment. 