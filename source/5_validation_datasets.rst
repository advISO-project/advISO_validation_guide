===========================================================================
Curating validation test datasets
===========================================================================

Principles
----------

As far as reasonably possible, test datasets should capture the fullest range of samples that the pipeline would be expected to encounter in its intended use. This should include straightforward cases as well as samples likely to challenge the pipeline, such as low quality or low input material, results close to a decision threshold, and known difficult scenarios relevant to the pipeline's application.

Challenges
----------

In practice, curating a validation dataset that meets the principles set out above is not always straightforward. Access to relevant samples, particularly rare or difficult cases, may be limited, and obtaining or generating them can carry significant cost. For many pipelines, no relevant external quality assessment scheme exists to provide independently characterised samples, leaving laboratories reliant on their own limited sample archives or, where available, samples shared through informal collaboration with other laboratories.

Possible solutions
------------------

**Simulated datasets**

Where real patient samples covering the full range of expected cases cannot be obtained, simulated data can supplement a validation dataset, for example by introducing known variants into real sequencing data at defined frequencies, or by simulating reads with defined characteristics. Simulated data allows edge cases and rare scenarios to be tested at known truth, but should not entirely replace real samples, since it cannot fully capture the technical and biological variability present in real world specimens.

To aid in the simulation of sequencing reads, the advISO project has developed a tool for simulating sequencing reads which is available on GitHub: https://github.com/advISO-project/pop_var_sim

**Data repositories**

Publicly available sequencing data held in repositories such as the European Nucleotide Archive can provide a source of validation material without the cost and delay of generating or obtaining new samples. Where data from such repositories is used, its provenance and the method by which it was originally characterised should be recorded, and its continued suitability for the pipeline's current intended use should be confirmed rather than assumed.

**Interlaboratory data sharing**

Where a laboratory does not hold sufficient samples of its own, arrangements with other laboratories, reference centres, or consortia can extend the range of validation material available, provided appropriate agreements are in place covering consent, data protection, and use.

**AdvISO validation datasets**

As part of the AdvISO project, a set of gold-standard validation datasets are currently under development for malaria, Mycobacterium tuberculosis (MTB), and HIV. These datasets combine real-world and simulated data with defined truth to support pipeline validation for these organisms.

- Malaria validation resources, including recipes for generating simulated datasets alongside real-world data, are available at advISO-project/validation_malaria.

- MTB validation resources are available at advISO-project/validation_data_MTB.

- An equivalent HIV validation dataset is currently under development.

These datasets are intended to reduce the access and cost barriers described in Section 5.2, providing laboratories with a shared, characterised resource rather than requiring each laboratory to independently source or generate validation material for these pathogens.