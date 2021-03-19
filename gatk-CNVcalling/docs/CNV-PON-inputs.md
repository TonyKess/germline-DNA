---
layout: default
title: "Inputs: PanelOfNormals"
---

# Inputs for PanelOfNormals

The following is an overview of all available inputs in
PanelOfNormals.


## Required inputs
<dl>
<dt id="PanelOfNormals.referenceFasta"><a href="#PanelOfNormals.referenceFasta">PanelOfNormals.referenceFasta</a></dt>
<dd>
    <i>File </i><br />
    The reference fasta file.
</dd>
<dt id="PanelOfNormals.referenceFastaDict"><a href="#PanelOfNormals.referenceFastaDict">PanelOfNormals.referenceFastaDict</a></dt>
<dd>
    <i>File </i><br />
    The sequence dictionary associated with the reference fasta file.
</dd>
<dt id="PanelOfNormals.referenceFastaFai"><a href="#PanelOfNormals.referenceFastaFai">PanelOfNormals.referenceFastaFai</a></dt>
<dd>
    <i>File </i><br />
    The index for the reference fasta file.
</dd>
</dl>

## Other common inputs
<dl>
<dt id="PanelOfNormals.annotateIntervals.mappabilityTrack"><a href="#PanelOfNormals.annotateIntervals.mappabilityTrack">PanelOfNormals.annotateIntervals.mappabilityTrack</a></dt>
<dd>
    <i>File? </i><br />
    Equivalent to gatk AnnotateIntervals' `--mappability-track` option.
</dd>
<dt id="PanelOfNormals.annotateIntervals.segmentalDuplicationTrack"><a href="#PanelOfNormals.annotateIntervals.segmentalDuplicationTrack">PanelOfNormals.annotateIntervals.segmentalDuplicationTrack</a></dt>
<dd>
    <i>File? </i><br />
    Equivalent to gatk AnnotateIntervals' `--segmenta-duplicarion-track` option.
</dd>
<dt id="PanelOfNormals.inputBamIndexes"><a href="#PanelOfNormals.inputBamIndexes">PanelOfNormals.inputBamIndexes</a></dt>
<dd>
    <i>Array[File] </i><i>&mdash; Default:</i> <code>[]</code><br />
    The indexes for the input BAM files.
</dd>
<dt id="PanelOfNormals.inputBams"><a href="#PanelOfNormals.inputBams">PanelOfNormals.inputBams</a></dt>
<dd>
    <i>Array[File] </i><i>&mdash; Default:</i> <code>[]</code><br />
    The BAM files for the samples to include in the PON. May be empty so just the annotated intervals can be created.
</dd>
<dt id="PanelOfNormals.outputDir"><a href="#PanelOfNormals.outputDir">PanelOfNormals.outputDir</a></dt>
<dd>
    <i>String </i><i>&mdash; Default:</i> <code>"."</code><br />
    The directory the output should be written to.
</dd>
<dt id="PanelOfNormals.PONname"><a href="#PanelOfNormals.PONname">PanelOfNormals.PONname</a></dt>
<dd>
    <i>String </i><i>&mdash; Default:</i> <code>"PON"</code><br />
    The name the PON file should be given.
</dd>
<dt id="PanelOfNormals.regions"><a href="#PanelOfNormals.regions">PanelOfNormals.regions</a></dt>
<dd>
    <i>File? </i><br />
    The regions to operate on.
</dd>
</dl>

## Advanced inputs
<details>
<summary> Show/Hide </summary>
<dl>
<dt id="PanelOfNormals.annotateIntervals.featureQueryLookahead"><a href="#PanelOfNormals.annotateIntervals.featureQueryLookahead">PanelOfNormals.annotateIntervals.featureQueryLookahead</a></dt>
<dd>
    <i>Int </i><i>&mdash; Default:</i> <code>1000000</code><br />
    Equivalent to gatk AnnotateIntervals' `--feature-query-lookahead` option
</dd>
<dt id="PanelOfNormals.annotateIntervals.intervalMergingRule"><a href="#PanelOfNormals.annotateIntervals.intervalMergingRule">PanelOfNormals.annotateIntervals.intervalMergingRule</a></dt>
<dd>
    <i>String </i><i>&mdash; Default:</i> <code>"OVERLAPPING_ONLY"</code><br />
    Equivalent to gatk AnnotateIntervals' `--interval-merging-rule` option.
</dd>
<dt id="PanelOfNormals.annotateIntervals.javaXmx"><a href="#PanelOfNormals.annotateIntervals.javaXmx">PanelOfNormals.annotateIntervals.javaXmx</a></dt>
<dd>
    <i>String </i><i>&mdash; Default:</i> <code>"2G"</code><br />
    The maximum memory available to the program. Should be lower than `memory` to accommodate JVM overhead.
</dd>
<dt id="PanelOfNormals.annotateIntervals.memory"><a href="#PanelOfNormals.annotateIntervals.memory">PanelOfNormals.annotateIntervals.memory</a></dt>
<dd>
    <i>String </i><i>&mdash; Default:</i> <code>"3G"</code><br />
    The amount of memory this job will use.
</dd>
<dt id="PanelOfNormals.annotateIntervals.timeMinutes"><a href="#PanelOfNormals.annotateIntervals.timeMinutes">PanelOfNormals.annotateIntervals.timeMinutes</a></dt>
<dd>
    <i>Int </i><i>&mdash; Default:</i> <code>5</code><br />
    The maximum amount of time the job will run in minutes.
</dd>
<dt id="PanelOfNormals.collectReadCounts.intervalMergingRule"><a href="#PanelOfNormals.collectReadCounts.intervalMergingRule">PanelOfNormals.collectReadCounts.intervalMergingRule</a></dt>
<dd>
    <i>String </i><i>&mdash; Default:</i> <code>"OVERLAPPING_ONLY"</code><br />
    Equivalent to gatk CollectReadCounts' `--interval-merging-rule` option.
</dd>
<dt id="PanelOfNormals.collectReadCounts.javaXmx"><a href="#PanelOfNormals.collectReadCounts.javaXmx">PanelOfNormals.collectReadCounts.javaXmx</a></dt>
<dd>
    <i>String </i><i>&mdash; Default:</i> <code>"7G"</code><br />
    The maximum memory available to the program. Should be lower than `memory` to accommodate JVM overhead.
</dd>
<dt id="PanelOfNormals.collectReadCounts.memory"><a href="#PanelOfNormals.collectReadCounts.memory">PanelOfNormals.collectReadCounts.memory</a></dt>
<dd>
    <i>String </i><i>&mdash; Default:</i> <code>"8G"</code><br />
    The amount of memory this job will use.
</dd>
<dt id="PanelOfNormals.collectReadCounts.timeMinutes"><a href="#PanelOfNormals.collectReadCounts.timeMinutes">PanelOfNormals.collectReadCounts.timeMinutes</a></dt>
<dd>
    <i>Int </i><i>&mdash; Default:</i> <code>1 + ceil((size(inputBam,"G") * 5))</code><br />
    The maximum amount of time the job will run in minutes.
</dd>
<dt id="PanelOfNormals.createReadCountPanelOfNormals.javaXmx"><a href="#PanelOfNormals.createReadCountPanelOfNormals.javaXmx">PanelOfNormals.createReadCountPanelOfNormals.javaXmx</a></dt>
<dd>
    <i>String </i><i>&mdash; Default:</i> <code>"7G"</code><br />
    The maximum memory available to the program. Should be lower than `memory` to accommodate JVM overhead.
</dd>
<dt id="PanelOfNormals.createReadCountPanelOfNormals.memory"><a href="#PanelOfNormals.createReadCountPanelOfNormals.memory">PanelOfNormals.createReadCountPanelOfNormals.memory</a></dt>
<dd>
    <i>String </i><i>&mdash; Default:</i> <code>"8G"</code><br />
    The amount of memory this job will use.
</dd>
<dt id="PanelOfNormals.createReadCountPanelOfNormals.timeMinutes"><a href="#PanelOfNormals.createReadCountPanelOfNormals.timeMinutes">PanelOfNormals.createReadCountPanelOfNormals.timeMinutes</a></dt>
<dd>
    <i>Int </i><i>&mdash; Default:</i> <code>5</code><br />
    The maximum amount of time the job will run in minutes.
</dd>
<dt id="PanelOfNormals.dockerImages"><a href="#PanelOfNormals.dockerImages">PanelOfNormals.dockerImages</a></dt>
<dd>
    <i>Map[String,String] </i><i>&mdash; Default:</i> <code>{"gatk": "broadinstitute/gatk:4.1.8.0"}</code><br />
    The docker images used. Changing this may result in errors which the developers may choose not to address.
</dd>
<dt id="PanelOfNormals.performExplicitGcCorrection"><a href="#PanelOfNormals.performExplicitGcCorrection">PanelOfNormals.performExplicitGcCorrection</a></dt>
<dd>
    <i>Boolean </i><i>&mdash; Default:</i> <code>true</code><br />
    Whether or not explicit GC correction should be used for PON generation. Setting this to false will also disable the creation of annotated intervals.
</dd>
<dt id="PanelOfNormals.preprocessIntervals.binLength"><a href="#PanelOfNormals.preprocessIntervals.binLength">PanelOfNormals.preprocessIntervals.binLength</a></dt>
<dd>
    <i>Int </i><i>&mdash; Default:</i> <code>if defined(intervals) then 0 else 1000</code><br />
    The size of the bins to be created. Should be 0 for targeted/exome sequencing.
</dd>
<dt id="PanelOfNormals.preprocessIntervals.intervalMergingRule"><a href="#PanelOfNormals.preprocessIntervals.intervalMergingRule">PanelOfNormals.preprocessIntervals.intervalMergingRule</a></dt>
<dd>
    <i>String </i><i>&mdash; Default:</i> <code>"OVERLAPPING_ONLY"</code><br />
    Equivalent to gatk PreprocessIntervals' `--interval-merging-rule` option.
</dd>
<dt id="PanelOfNormals.preprocessIntervals.javaXmx"><a href="#PanelOfNormals.preprocessIntervals.javaXmx">PanelOfNormals.preprocessIntervals.javaXmx</a></dt>
<dd>
    <i>String </i><i>&mdash; Default:</i> <code>"3G"</code><br />
    The maximum memory available to the program. Should be lower than `memory` to accommodate JVM overhead.
</dd>
<dt id="PanelOfNormals.preprocessIntervals.memory"><a href="#PanelOfNormals.preprocessIntervals.memory">PanelOfNormals.preprocessIntervals.memory</a></dt>
<dd>
    <i>String </i><i>&mdash; Default:</i> <code>"4G"</code><br />
    The amount of memory this job will use.
</dd>
<dt id="PanelOfNormals.preprocessIntervals.padding"><a href="#PanelOfNormals.preprocessIntervals.padding">PanelOfNormals.preprocessIntervals.padding</a></dt>
<dd>
    <i>Int </i><i>&mdash; Default:</i> <code>if defined(intervals) then 250 else 0</code><br />
    The padding to be added to the bins. Should be 0 if contiguos binning is used, eg with WGS.
</dd>
<dt id="PanelOfNormals.preprocessIntervals.timeMinutes"><a href="#PanelOfNormals.preprocessIntervals.timeMinutes">PanelOfNormals.preprocessIntervals.timeMinutes</a></dt>
<dd>
    <i>Int </i><i>&mdash; Default:</i> <code>1 + ceil((size(referenceFasta,"G") * 6))</code><br />
    The maximum amount of time the job will run in minutes.
</dd>
</dl>
</details>




