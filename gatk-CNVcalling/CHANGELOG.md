Changelog
==========

<!--

Newest changes should be on top.

This document is user facing. Please word the changes in such a way
that users understand how the changes affect the new version.
-->

version 1.1.0
---------------------------
+ Update default GATK image to 4.1.8.0.
+ Tasks were updated to contain the `time_minutes` runtime attribute and
  associated `timeMinutes` input, describing the maximum time the task will
  take to run.

version 1.0.0
---------------------------
+ Added input for minimum contig length
+ Added `commonVariantSitesIndex` input
+ Added documentation
+ Added pairedCnvCalling.wdl and sample.wdl
+ Added CNV-PON.wdl
