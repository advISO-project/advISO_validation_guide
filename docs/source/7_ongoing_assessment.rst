.. _ongoing-assessment:

===========================================================================
Assessing Ongoing Fitness for Purpose
===========================================================================

Validation at the point of implementation provides evidence that a pipeline delivers the required performance criteria at that time, but it does not guarantee that the pipeline remains fit for purpose throughout its ongoing use. As outlined in Section 2, ISO 151
89 requires that laboratories have a process in place to monitor ongoing fitness for purpose. This may involve checking fitness for purpose following a specific change to the pipeline or its dependencies, or monitoring performance over time in the absence of any identified change, in order to detect drift that develops gradually rather than as the result of a single event.

----------------------------------------------------------------------------------------------

Verification and revalidation triggers
--------------------------------------

A defined set of triggers should be established to identify when a pipeline requires verification or revalidation, rather than relying on this being identified informally. Triggers may include changes to the pipeline's code or configuration, updates to reference databases or annotation sources, changes to the version of underlying software or tools used within the pipeline, and changes to the sequencing platform or wet laboratory protocol that generates the data the pipeline processes. Triggers may also include changes to the clinical or public health use case the pipeline supports, or to the intended population it is applied to, since a change in use case can alter the performance criteria the pipeline is required to meet. In addition to these change based triggers, periodic monitoring through regression testing, in which the pipeline is run at defined intervals against its existing validation dataset or a fixed set of reference samples, allows performance to be confirmed as stable over time and can surface drift not captured by an identifiable change.

----------------------------------------------------------------------------------------------

Deciding between verification and full revalidation
---------------------------------------------------

Not every trigger identified in Section 7.1 requires a pipeline to be revalidated in full. Whether verification or full revalidation is appropriate should be determined by the scale of the change and its likely impact on the pipeline's established performance characteristics.

Verification is appropriate where a change is not expected to affect the pipeline's analytical performance, but confirmation is nonetheless required to demonstrate that this is the case. This applies, for example, to peripheral or downstream changes, such as an update to reporting format, a change to compute infrastructure that does not alter the analytical method, or a minor version update to a dependency that does not change the algorithm's behaviour. Verification typically involves confirming that the pipeline continues to produce the expected results on a defined subset of the original validation dataset, or on known reference samples, without repeating the full validation process.

Full revalidation is required where a change has the potential to alter the pipeline's analytical performance characteristics, or where the scale or nature of the change cannot be confidently assessed through a limited check alone. This applies, for example, to a change in the underlying algorithm or analytical method, a change to the reference database or annotation source against which results are called, a change to the sequencing platform or wet laboratory protocol generating the input data, or a change to the clinical use case or intended population the pipeline supports. In each of these cases, the change directly affects the basis on which the pipeline's original performance criteria were established.

Where it is unclear whether a change warrants verification or full revalidation, the more rigorous option should be applied. The rationale for this decision should be documented at the time it is made, rather than reconstructed afterward, consistent with the traceability principle established earlier in this guide.
