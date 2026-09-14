===========================================================================
Pre-established Performance Criteria
===========================================================================

As established in the previous section, validation requires objective evidence that pre-established performance criteria have been met before an examination method is adopted. For this reason, the first step in the development of any bioinformatics pipeline should be to define the clinical (or public health) question that it is intended to answer, and to establish the performance criteria required to confidently answer that question. This should happen before any code is written.

Defining the clinical question first, rather than beginning with building the pipeline, ensures that performance criteria are set according to the decision a result will be used to support, rather than being derived retrospectively from what the pipeline happens to achieve. A pipeline built without this step risks being validated against criteria that describe its own output rather than the requirements of its intended use, an approach that provides no objective assurance that the pipeline is fit for purpose.

Questions to consider when defining performance criteria
--------------------------------------------------------

When defining performance requirements for an examination method, the following questions should be considered based on the consequences of an incorrect result:

**What is the clinical impact of a false negative?**

In situations where a false negative would deny a patient timely access to tailored treatments, the sensitivity threshold required for pipeline acceptance should be set high in proportion to the severity of that impact. Examples could include missing targetable somatic variants that would have indicated eligibility for mutation-specific targeted cancer therapies, or missing a resistance mutation that would otherwise have indicated the need for a more effective HIV antiretroviral regimen. In both of these examples, a false negative results in a patient not receiving the treatment most likely to be effective for their disease.

**What is the clinical impact of a false positive?**

In situations where a false positive would result in a patient undergoing unnecessary treatment, investigation, or intervention, with no clinical benefit and potentially additional harm or burden as a result, the specificity threshold required for pipeline acceptance should be set proportionally high. Examples could include an incorrectly identified pathogenic BRCA variant resulting in a patient being recommended preventative surgery, or a false positive resistance mutation resulting in a patient being switched to a treatment with greater side effects than the regimen that would otherwise have been effective.

**Is the clinical decision based on the pipeline’s results reversible?**

Some decisions based on an incorrect result, such as moving a patient to a more frequent screening regime following a false positive, can be corrected with limited harm. For example, that patient can be switched back to a standard screening frequency once the result is clarified, with the additional screening representing a manageable burden rather than a lasting harm. Other decisions based on incorrect results e.g. surgical intervention or initiation of an irreversible treatment cannot be undone. When decisions based on the results of a pipeline are irreversible, performance criteria should be set stringently as to minimise the likelihood of an error causing harm that cannot be subsequently corrected.

**How urgently are decisions made following a pipeline result?**

Some results demand immediate action, allowing little time to identify an error before the result feeds into clinical decision making. For example, genetic testing prior to cancer treatment often requires tight turnaround times, where a treatment decision must be make quickly following diagnosis, and therefore there is limited opportunity for interrogation of results. Acutely unwell children represent a similarly urgent context, where a bioinformatics result (e.g. from rapid whole genome trio testing) may need to inform treatment within hours, leaving no time for erroneous results to be identified through parallel or follow up processes before clinical action is taken. In both these cases, the absence of time to catch an error before it affects patient management means that performance criteria for pipelines supporting these decisions should be set to the highest achievable standard prior to deployment.

**What is the position of the pipeline in the wider testing pathway?**

Where clinical decisions are made on the basis of a bioinformatics pipeline result alone, stricter performance criteria thresholds should be set compared to when pipeline results are considered alongside the results of other tests (e.g. confirmatory testing following a positive public health screening test to rule out false positives) or the patient's clinical presentation. These provide an independent opportunity to identify and correct an erroneous result before a decision is acted on.