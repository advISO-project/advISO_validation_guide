===========================================================================
Scope and Definitions
===========================================================================

Intended audience
-----------------

This guidance has been written with clinical/public health laboratories in mind to aid them to perform validation of bioinformatics pipelines as part of the requirements set out in ISO 15189. However, it is equally of use to those working outside of ISO 15189 accredited laboratories. For example, currently unaccredited laboratories considering applying for accreditation in the future, or research institutions developing bioinformatics pipelines that they hope to be adopted by clinical laboratories.

Validation vs. Verification
---------------------------

Many laboratories use the terms ‘validation’ and ‘verification’ interchangeably; however within ISO 15189 these are separate and distinct processes triggered by different circumstances.

**What is validation?**

Validation is the confirmation, through the provision of objective evidence, that an examination method is fit for its specific intended use. This is achieved by establishing and documenting the examination method's performance characteristics and comparing these against pre-defined acceptance criteria derived from the requirements of the intended use case. Ascertaining the performance characteristics of an examination method typically involves assessing accuracy, precision (repeatability and reproducibility), sensitivity and specificity, limits of detection, and reportable range of results (see Table 1 for definitions). Broadly speaking, validation can be distilled into two main questions:

1. What are the performance characteristics of the examination method?
2. Do the performance characteristics meet the requirements for the examination method’s intended use?

Validation applies where an examination method has not been previously validated for the laboratory’s intended use. In a bioinformatics context this could include in-house developed pipelines/software/databases or when externally validated pipelines/software/databases are used outside of their intended scope.

**What is verification?**

In contrast, verification is the process of confirming that an examination method’s performance criteria continue to meet the requirements for its intended use. Verification is therefore primarily concerned with the question *“Are the performance characteristics still the same, given a change to the method itself or to the operating context in which it is used?”*.

Verification applies in two circumstances:

1. When a laboratory adopts an examination method already validated by an external source (e.g. a commercially available pipeline or a pipeline developed by a third-party) without modification. Here verification confirms the laboratory can reproduce the established performance using its own equipment and staff.

2. When an in-house examination method, previously validated by the laboratory, has since undergone modification that is minor in extent (see section on assessing the impact of pipeline changes). Here the role of verification is to check that the update to the examination method has not negatively affected the performance criteria of the examination method, and that it remains fit for clinical purpose. 

Definitions
-----------

Below are definitions of the performance characteristics that are typically assessed during validation of a bioinformatics pipeline.

.. dropdown:: Accuracy

    The ability of a pipeline to produce accurate results. Accuracy is assessed by processing samples of known or reference-confirmed characteristics through the pipeline, and comparing the resulting output against that established truth.

.. dropdown:: Limits of detection

    The lowest concentration of an analyte that can be reliably detected. In a bioinformatics context this may include the minimum frequency at which a variant can be reliably detected/distinguished from sequencing error.

.. dropdown:: Precision

    The ability of a pipeline to produce consistent results when applied repeatedly, either under unchanged conditions or across independent sample preparations. The two core components of precision include repeatability and reproducibility (see below).

.. dropdown:: Repeatability

    The ability of a pipeline to produce repeatable results using the same input data. Repeatability is assessed by processing the same input data through the pipeline multiple times under unchanged conditions (i.e. same code version, software environment, parameters, and reference datasets) and comparing results (e.g. variant concordance, lineage assignment concordance, AMR gene call concordance etc.). Because the input and configuration are held constant, any variation observed reflects non-determinism intrinsic to the pipeline itself e.g. unseeded stochastic algorithms, floating-point non-associativity in parallelised computation, or race conditions in multi-threaded execution). 

.. dropdown:: Reproducibility

    The ability of a pipeline to produce concordant results across independent sample preparations. Reproducibility is assessed by running independent library preps / sequencing replicates of the same sample through the pipeline, and measuring concordance of the output calls (e.g. variant concordance, lineage assignment concordance, AMR gene calls) between replicates. Because replicates diverge upstream of the analytical pipeline, this measure captures precision of the combined wet-lab and bioinformatic workflow rather than the pipeline in isolation.

.. dropdown:: Sensitivity

    The proportion of true positives correctly identified by an examination method. High sensitivity is required for screening tests, in order to minimise false negatives, which is important in contexts where a missed positive result carries a significant clinical or public health cost.

.. dropdown:: Specificity

    The proportion of true negatives correctly identified by an examination method. High specificity is required for diagnostic tests in order to minimise false positives, which is important where an incorrect positive result would lead to unnecessary treatment.

.. dropdown:: Reportable range

    The ability of a pipeline to produce valid, clinically or epidemiologically meaningful results across the full span of input conditions it may encounter in use. Reportable range is assessed by processing samples that span the expected extremes of relevant input variables (e.g. sequencing depth/coverage, sample quality, sample types, pathogen load, tumour content etc.) through the pipeline, and determining the boundaries within which output calls remain valid.

Additional definitions of ISO 15189 terms are provided in the `glossary of terms <https://adviso-sop-guide.readthedocs.io/en/latest/glossary.html>`_ section of our SOP writing Guide.
