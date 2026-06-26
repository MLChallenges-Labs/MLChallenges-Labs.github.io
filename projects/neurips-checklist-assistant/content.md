## Overview

We are excited to announce a study to understand if Large Language Models (LLMs) can serve as an assistant to help authors verify their submission against the NeurIPS Paper Checklist. This study is a first step towards understanding if LLMs can be used to enhance the quality of submissions at NeurIPS. We invite authors intending to submit a paper to NeurIPS to participate in this study by pre-registering through our online form, before the abstract submission deadline. Participants will gain access to an experimental LLM assistant (on or shortly before the abstract submission deadline), which will provide feedback on if their paper submission complies with NeurIPS submission standards, and are asked to fill out two short surveys describing their experiences with the LLM assistant. Due to limited computational resources, participation may be limited, and will be offered on a first-come, first-served basis.

## Why This Matters

The NeurIPS Paper Checklist is a series of yes/no questions that help authors check if their work meets reproducibility, transparency, and ethical research standards expected for papers at NeurIPS, and is a critical component in maintaining the high standards of research presented at the conference. By ensuring that submissions adhere to this checklist, we uphold the scientific rigor and transparency that NeurIPS aims for.

Currently, some authors might already be using LLMs as tools in their research and writing processes. While the wider ethical implications and appropriate use cases of LLMs remain unclear and must be a larger community discussion, here, we evaluate a more clear-cut and low-risk use case: vetting paper submissions against submission standards, with results shown only to the authors. Our aim is to systematically evaluate the benefits and risks of LLMs, by conducting a structured study to understand if LLMs can enhance research quality and improve efficiency by helping authors understand if their work meets research standards like the NeurIPS Paper Checklist. This study will test the effectiveness of LLMs in an academic publishing setting, and potentially influence broader AI applications in research evaluation.

## How It Works

The LLM assistant is hosted by ChaLearn on Codabench.org. We invite NeurIPS authors to try out the assistant for their papers, and fill out two brief surveys.

- **Registration:** For any paper, a single delegated author should register at this link. Due to a limited budget, participation will be offered on a first come first served basis. Registered participants will receive an invitation to the assistant's page on the Codabench platform, and will need to create an account on Codabench using the email supplied in the registration.
- **Submissions:** Submissions are entirely optional and completely separate from the NeurIPS paper submission system and the review process. Papers must be formatted as specified in the NeurIPS'24 CFP (complete with appendices and checklist). Information provided in external links will not be taken into account by the assistant. We ask submitters to fill out the checklist to the best of their abilities.
- **Anonymity and confidentiality:** Authors can retain their anonymity by registering to Codabench with an email and login that do not reveal their identity, and by submitting anonymized papers. The papers and LLM outputs will be kept confidential and will not be accessible to NeurIPS reviewers, ACs, and PCs. Only aggregated statistics will be published, after the review process is over. It is important to note that while authors retain ownership of their submissions, the papers will be sent to the API of an LLM service, and treated under their conditions of confidentiality.

## The Role of the Assistant

The LLM Assistant will provide detailed feedback on whether the responses to the checklist questions accompanying the paper are satisfactory. This feedback is intended to guide authors in refining their papers before official submission. Please remember that this tool is designed to supplement, not replace, critical judgment and expertise. In particular, it is certainly possible for the review process to raise concerns about the checklist that have not been raised by the LLM reviews.

Here are some examples of feedback (for two different papers). Green means that the LLM assistant has identified no significant concerns. Yellow means that the LLM assistant has identified an inconsistency with NeurIPS Paper Checklist standards, and authors are encouraged to validate the issue identified by the LLM assistant and make any necessary improvements.

**Question #3:** For each theoretical result, does the paper provide the full set of assumptions and a complete (and correct) proof?

*Author's answer:* No

*Author's justification:* There is no theory in this paper.

*LLM Review:* The answer provided by the authors is consistent with the content of the paper. Based on the detailed review of the paper, it is clear that the work primarily focuses on conducting an observational study to investigate the presence of citation bias in peer review processes. The study utilizes statistical modeling and analysis rather than theoretical developments that would involve theorems, lemmas, or formal proofs. Therefore, the classification of the answer as "NA" (Not Applicable) is accurate given the nature of the research presented. However, to provide constructive and actionable suggestions for improvement and to ensure thorough and critical assessment, it is beneficial to clearly outline the assumptions behind the statistical models and analyses employed. This would enhance the readability and understandability of the study's methodology and its limitations. [...]

---

**Question #12:** Are the creators or original owners of assets (e.g., code, data, models), used in the paper, properly credited and are the license and terms of use explicitly mentioned and properly respected?

*Author's answer:* Yes.

*Author's justification:* We have used algorithms such as TPMS and PeerReview4All. We have cited them.

*LLM Review:* There does not appear to be any discrepancy between the authors' justification for the cited question and the actual paper content in terms of providing proper credit and mentioning licenses for used assets, according to their statement. However, the detailed source citations such as the specific papers for TPMS (Toronto Paper Matching System) and PeerReview4All, including their licenses or terms of use, are not explicitly mentioned in the provided text. It's essential to ensure that these aspects are clearly attributed and any terms of use are respected, as stated in the initial guidelines provided to authors. [...]

## Limitations, Disclaimer and Final Thoughts

Despite advances in AI, LLMs still face several limitations when used in verifying scientific submissions. LLMs may misinterpret complex content or fail to fully assess checklist criteria, leading to verification errors. There is also a risk that authors might rely too much on the LLM analysis, potentially missing deeper issues that require human judgment. We encourage authors to manually validate the outputs of LLMs, and to use the tool to supplement their judgment, not replace it. Known issues include false positives (e.g., LLM may ask for extra justifications or changes that are excessive or irrelevant) as well as false negatives (e.g., the LLM overlooks errors in proofs). As of the release of this blog, the LLM answers are based only on the text of the paper and does not check figures, tables, and external links (such as Github repos), hence it may complain about missing information that is found in those assets.

Additionally, using LLMs raises concerns about data privacy and security, as papers are processed through an LLM service API. We provide recommendations to participants on anonymizing their submissions and we are making best efforts to keep all papers in confidence. However, we decline responsibility on possible unintentional leaks of data, due to mishandling or due to the use of a third party LLM. If authors are concerned for the security of their paper, we do not recommend them to participate in the study.

Limited computational resources mean only some authors can access this service, possibly creating unequal opportunities. Furthermore, inherent biases in LLMs could compromise the fairness and impartiality of the process, especially for unconventional or interdisciplinary research. We mitigate these risks by only providing this tool to authors with the intention of feedback: the outputs of the LLM will not be visible to, or used by reviewers, ACs, and PCs in their review of the submission.

This study is strictly for educational and research purposes. The organizers, sponsors, and NeurIPS assume no liability for any direct or indirect consequences arising from participation. Authors are reminded to use their discretion and adhere to all NeurIPS guidelines when submitting their papers to OpenReview for official review.

## Credits

The principal organizers of this experiment are: Ihsan Ullah, Alexander Goldberg, Isabelle Guyon, Thanh Gia Hieu Khuong, Benedictus Kent Rachmat, Nihar Shah, and Zhen Xu.

In preparing this experiment, we received advice and help from many people. We are particularly grateful to the NeurIPS'24 organizers, including General Chair Amir Globerson, Program Chairs Danielle Belgrave, Cheng Zhang, Angela Fan, Jakub Tomczak, Ulrich Paquet, and workflow team member Babak Rahmani, for participating in brainstorming discussions and contributing to the design. We have also received inputs and encouragement from Andrew McCallum of OpenReview, Anurag Acharya from Google Scholar, and Tristan Neuman from the NeurIPS board. Several volunteers have contributed ideas and helped with various aspects of the preparation, including Jeremiah Liu, Lisheng Sun, Paulo Henrique Couto, Michael Brenner, Neha Nayak Kennard, and Adrien Pavao.

We are grateful to Marc Schoenauer for supporting this effort with an INRIA Google Research grant. We acknowledge the support of ChaLearn and of the ANR Chair of Artificial Intelligence HUMANIA ANR-19-CHIA-0022.

## References

Competition website: [Link](https://www.codabench.org/competitions/2338/)

NeurIPS Blog: [Link](https://blog.neurips.cc/2024/05/07/soliciting-participants-for-the-neurips-2024-checklist-assistant-study/)
