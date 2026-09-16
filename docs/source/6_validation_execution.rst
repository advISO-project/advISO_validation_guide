===========================================================================
Peforming a Validation
===========================================================================

Once a validation plan has been approved, in accordance with Section 4, testing can proceed. This section sets out the expectations for good scientific practice during testing, how results should be recorded, and how the outcome should be reported and signed off before the pipeline is deployed for use.

----------------------------------------------------------------------------------------------

Good scientific practice
------------------------

Validation testing should follow the approved plan, using the methods, dataset and criteria specified in advance . Any deviation from the plan should be documented, along with the reason for the deviation and its potential impact on the results. Testing should be performed by, or supervised by, an appropriately qualified individual. The version of the pipeline under test, along with the reference databases, software dependencies and compute environment used, should be recorded so the validation is reproducible and can be tied to a defined pipeline state.

----------------------------------------------------------------------------------------------

Storing results
---------------

Raw outputs, intermediate files and summary results generated during validation should be retained in line with the laboratory's data retention policy, and should remain accessible for as long as needed to support the validation report and any later audit or review. Where storing full raw outputs is not practical, a defined subset or summary sufficient to support the conclusions of the validation should be retained instead, with the reasoning documented.

----------------------------------------------------------------------------------------------

Validation report
-----------------

On completion of testing, a validation report should be produced, setting out the evidence gathered and the conclusion reached on whether the pipeline is fit for its intended purpose. A validation report should cover the following:

.. dropdown:: Project summary
    
    A brief description of the pipeline, the clinical or public health question it addresses, and the intended use population, providing the reader with the context needed to interpret the rest of the report.

.. dropdown:: Requirements, risk assessment and qualification
    
    Covers the user requirements specification, functional specification, and risk assessment carried out to define what the pipeline needs to do and the performance criteria required of it, along with installation qualification and operational qualification confirming the pipeline has been correctly installed and operates as intended in its deployment environment.

.. dropdown:: Performance qualification and results
    
    Presents the results of testing against the pre established performance criteria, including sensitivity, specificity, and other relevant metrics, together with the limit of detection determined during validation.

.. dropdown:: Quality assurance evidence
    
    Summarises the internal quality control, internal quality assessment, and external quality assessment evidence, where available, that supports ongoing confidence in the pipeline's performance beyond the point of validation itself.

.. dropdown:: SOP, training and infrastructure
    
    Confirms that a standard operating procedure has been developed and that relevant staff have received and recorded training on the pipeline, alongside evidence of the compute infrastructure, backup arrangements, and code review practices supporting its ongoing maintenance.

.. dropdown:: Summary and recommendation
    
    Draws together the evidence presented and states whether the pipeline is fit for its intended purpose, including whether its implementation requires notification of users or an application for extension to scope.

.. dropdown:: Report sign off
    
    Records formal approval of the report by an appropriately authorised individual, confirming the pipeline is approved for deployment.

----------------------------------------------------------------------------------------------

Independent review and report sign off prior to pipeline deployment
-------------------------------------------------------------------

The validation report should undergo independent technical review before sign off. This means an appropriately qualified individual, not directly involved in performing the validation, checks that the results support the stated conclusion and that testing followed the approved plan. Following technical review, the report should be formally signed off by an appropriately authorised individual, confirming approval for the pipeline to be deployed for its intended use. Where the same individual carries out both technical review and sign off, this should be justified and recorded, since separating the two roles gives a stronger safeguard against an error going unnoticed. Sign off should be recorded along with the name and role of the signatory, or signatories, and the date of approval. The validation report should be stored within the laboratory's quality management system.

----------------------------------------------------------------------------------------------

Handling validation failure
---------------------------

Where a pipeline does not meet its pre established performance criteria, this should be recorded in the validation report in the same manner as a successful validation, together with an assessment of why the criteria were not met. The pipeline should not be deployed for the use case it was validated against until the deficiency has been addressed and validation repeated, unless a restricted scope of use can be justified and independently approved, in which case the basis for that restriction should be clearly documented. A failed validation should feed back into pipeline development, and where relevant, into the performance criteria or validation plan themselves, if the failure suggests these were not appropriately set.