===========================================================================
Developing a Validation Plan
===========================================================================

Ahead of validating a pipeline against pre-established performance requirements, a detailed plan for performing the validation should be prepared and agreed to set out how pipeline performance will be assessed. Having a validation plan ensures that (1) testing is conducted systematically; (2) acceptance decisions are made objectively against thresholds agreed in advance; and (3) the process is both traceable and reproducible. Without a validation plan, there is a risk that testing is conducted inconsistently, that acceptance criteria are adjusted after results are seen, or that the basis on which a pipeline was judged fit for purpose cannot later be reconstructed or defended.

----------------------------------------------------------------------------------------------

What should be included in a validation plan?
---------------------------------------------

A validation plan should include the following elements:

.. dropdown:: Summary and rationale for chosen methods

    A brief summary of the pipeline, the clinical or public health question it is intended to answer, the intended sample/data types it will process, and a rationale for the chosen method(s) i.e. why each approach, algorithm, software, reference etc was selected over other available alternatives, and how it is expected to meet the perform criteria.

.. dropdown:: Validation dataset

    A description of the dataset(s) against which the pipeline will be tested, including their provenance, and justification that they are representative of the intended use population and the range of samples pipeline will encounter in practice, including relevant positive, negative, and edge cases. Where reference materials or established truth sets are limited, the plan should describe how this limitation was addressed and what assumptions or compromises were made.

    For further guidance on the curation of validation test datasets see :ref:`Curating Validation Test Datasets section <curating-validation-test-datasets>`. 

.. dropdown:: What will be measured and how

    The specific performance metrics to be assessed, e.g. sensitivity, specificity, positive and negative predictive value, or limit of detection, together with the method by which each will be calculated.

.. dropdown:: Minimum acceptance criteria

    The pre-defined acceptance thresholds for each performance metric, along with a clear statement of what constitutes a pass or fail against each.

.. dropdown:: Schedule of activities

    A timeline setting out the sequence in which validation activities and other key milestones (e.g. SOP development) will be completed.

.. dropdown:: Approval

    Before validation activities commence, the validation plan itself should be reviewed and formally approved by someone independent of its preparation. This independent review provides assurance that the proposed assessment methods (and validation dataset) are appropriate and sufficiently rigorous for the pipeline's intended use before any testing begins. Approval of the plan should be formally recorded, together with the name and role of the approver and the date of approval, ensuring traceability of the decision-making process before validation testing proceeds.