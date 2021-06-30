# Knowledge-grounded Retrieval-based Chatbots

Knowledge-grounded response selection in retrieval-based chatbot is a task which aims to select the most suitable response from a set of candidates. The selected response should be not only coherent with the context but also consistent with the given knowledge. The knowledge here is usually represented by documents. This task is attracting more and more attention in both academia and industry. However, no one has maintained a leaderboard and a collection of popular papers and datasets yet. The main objective of this repository is to provide a quick overview of benchmark datasets and the state-of-the-art studies on this task.

## Datasets

### Persona-chat
- [Zhang et al.](https://github.com/facebookresearch/ParlAI/tree/master/projects/personachat) released the original version. [[download]](https://github.com/facebookresearch/ParlAI/tree/mturk_archive)
- [Gu et al.](https://www.aclweb.org/anthology/2020.findings-emnlp.127.pdf) released a version with vocabulary and embeddings. [[download]](https://github.com/JasonForJoy/FIRE)

### CMUDoG
- [Zhou et al.](https://arxiv.org/pdf/1809.07358.pdf) released the original version. [[download]](https://github.com/festvox/datasets-CMU_DoG)
- [Gu et al.](https://www.aclweb.org/anthology/2020.findings-emnlp.127.pdf) released a version with vocabulary and embeddings. [[download]](https://github.com/JasonForJoy/FIRE)

## Leaderboard

### Persona-chat-Original

| Model                    |   R@1   |   R@2   |   R@5   |   Paper and Code   |
| ------------------------ | ------- | ------- | ------- | ------------------ |
| Starspace                |   49.1  |   60.2  |   76.5  | StarSpace: Embed All The Things!. AAAI 2018. [[paper]](https://arxiv.org/pdf/1709.03856.pdf) [[code]](https://github.com/facebookresearch/StarSpace)|
| Profile                  |   50.9  |   60.7  |   75.7  | Personalizing Dialogue Agents: I have a dog, do you have pets too?. ACL 2018. [[paper]](https://www.aclweb.org/anthology/P18-1205.pdf) [[code]](https://github.com/facebookresearch/ParlAI/tree/master/projects/personachat)|
| KV Profile               |   51.1  |   61.8  |   77.4  | Personalizing Dialogue Agents: I have a dog, do you have pets too?. ACL 2018. [[paper]](https://www.aclweb.org/anthology/P18-1205.pdf) [[code]](https://github.com/facebookresearch/ParlAI/tree/master/projects/personachat)|
| Transformer              |   54.2  |   68.3  |   83.8  | Training Millions of Personalized Dialogue Agents. EMNLP 2018. [[paper]](https://www.aclweb.org/anthology/D18-1298.pdf)|
| DGMN                     |   67.6  |   80.2  |   92.9  | A Document-grounded Matching Network for Response Selection in Retrieval-based Chatbots. IJCAI 2019. [[paper]](https://arxiv.org/pdf/1906.04362.pdf)|
| DIM                      |   78.8  |   89.5  |   97.0  | Dually Interactive Matching Network for Personalized Response Selection in Retrieval-Based Chatbots. EMNLP 2019. [[paper]](https://www.aclweb.org/anthology/D19-1193.pdf) [[code]](https://github.com/JasonForJoy/DIM)|
| CSN                      |   78.1  |   89.0  |   97.1  | Content Selection Network for Document-grounded Retrieval-based Chatbots. ECIR 2021. [[paper]](https://arxiv.org/pdf/2101.08426.pdf) [[code]](https://github.com/DaoD/CSN)|
| RSM-DCK                  |   79.7  |   90.2  |   97.5  | Learning to Detect Relevant Contexts and Knowledge for Response Selection in Retrieval-based Dialogue Systems. CIKM 2020. [[paper]](https://dl.acm.org/doi/pdf/10.1145/3340531.3411967)|
| FIRE                     |   81.6  |   91.2  |   97.8  | Filtering before Iteratively Referring for Knowledge-Grounded Response Selection in Retrieval-Based Chatbots. EMNLP 2020: Findings. [[paper]](https://www.aclweb.org/anthology/2020.findings-emnlp.127.pdf) [[code]](https://github.com/JasonForJoy/FIRE)|
| MNDB                     |   75.6  |   86.9  |   95.7  | Adapting to Context-Aware Knowledge in Natural Conversation for Multi-Turn Response Selection. WWW 2021. [[paper]](https://dl.acm.org/doi/pdf/10.1145/3442381.3449902)|

### Persona-chat-Revised

| Model                    |   R@1   |   R@2   |   R@5   |   Paper and Code   |
| ------------------------ | ------- | ------- | ------- | ------------------ |
| Starspace                |   32.2  |   48.3  |   66.7  | StarSpace: Embed All The Things!. AAAI 2018. [[paper]](https://arxiv.org/pdf/1709.03856.pdf) [[code]](https://github.com/facebookresearch/StarSpace)|
| Profile                  |   35.4  |   48.3  |   67.5  | Personalizing Dialogue Agents: I have a dog, do you have pets too?. ACL 2018. [[paper]](https://www.aclweb.org/anthology/P18-1205.pdf) [[code]](https://github.com/facebookresearch/ParlAI/tree/master/projects/personachat)|
| KV Profile               |   35.1  |   45.7  |   66.3  | Personalizing Dialogue Agents: I have a dog, do you have pets too?. ACL 2018. [[paper]](https://www.aclweb.org/anthology/P18-1205.pdf) [[code]](https://github.com/facebookresearch/ParlAI/tree/master/projects/personachat)|
| Transformer              |   42.1  |   56.5  |   75.0  | Training Millions of Personalized Dialogue Agents. EMNLP 2018. [[paper]](https://www.aclweb.org/anthology/D18-1298.pdf)|
| DGMN                     |   58.8  |   62.5  |   87.7  | A Document-grounded Matching Network for Response Selection in Retrieval-based Chatbots. IJCAI 2019. [[paper]](https://arxiv.org/pdf/1906.04362.pdf)|
| DIM                      |   70.7  |   84.2  |   95.0  | Dually Interactive Matching Network for Personalized Response Selection in Retrieval-Based Chatbots. EMNLP 2019. [[paper]](https://www.aclweb.org/anthology/D19-1193.pdf) [[code]](https://github.com/JasonForJoy/DIM)|
| CSN                      |   71.3  |   84.0  |   95.5  | Content Selection Network for Document-grounded Retrieval-based Chatbots. ECIR 2021. [[paper]](https://arxiv.org/pdf/2101.08426.pdf) [[code]](https://github.com/DaoD/CSN)|
| RSM-DCK                  |   71.9  |   84.9  |   95.5  | Learning to Detect Relevant Contexts and Knowledge for Response Selection in Retrieval-based Dialogue Systems. CIKM 2020. [[paper]](https://dl.acm.org/doi/pdf/10.1145/3340531.3411967)|
| FIRE                     |   74.8  |   86.9  |   95.9  | Filtering before Iteratively Referring for Knowledge-Grounded Response Selection in Retrieval-Based Chatbots. EMNLP 2020: Findings. [[paper]](https://www.aclweb.org/anthology/2020.findings-emnlp.127.pdf) [[code]](https://github.com/JasonForJoy/FIRE)|
| MNDB                     |   73.6  |   83.0  |   95.2  | Adapting to Context-Aware Knowledge in Natural Conversation for Multi-Turn Response Selection. WWW 2021. [[paper]](https://dl.acm.org/doi/pdf/10.1145/3442381.3449902)|


### CMUDoG

| Model                    |   R@1   |   R@2   |   R@5   |   Paper and Code   |
| ------------------------ | ------- | ------- | ------- | ------------------ |
| Starspace                |   50.7  |   64.5  |   80.3  | StarSpace: Embed All The Things!. AAAI 2018. [[paper]](https://arxiv.org/pdf/1709.03856.pdf) [[code]](https://github.com/facebookresearch/StarSpace)|
| Profile                  |   51.6  |   65.8  |   81.4  | Personalizing Dialogue Agents: I have a dog, do you have pets too?. ACL 2018. [[paper]](https://www.aclweb.org/anthology/P18-1205.pdf) [[code]](https://github.com/facebookresearch/ParlAI/tree/master/projects/personachat)|
| KV Profile               |   56.1  |   69.9  |   82.4  | Personalizing Dialogue Agents: I have a dog, do you have pets too?. ACL 2018. [[paper]](https://www.aclweb.org/anthology/P18-1205.pdf) [[code]](https://github.com/facebookresearch/ParlAI/tree/master/projects/personachat)|
| Transformer              |   60.3  |   74.4  |   87.4  | Training Millions of Personalized Dialogue Agents. EMNLP 2018. [[paper]](https://www.aclweb.org/anthology/D18-1298.pdf)|
| DGMN                     |   65.6  |   78.3  |   91.2  | A Document-grounded Matching Network for Response Selection in Retrieval-based Chatbots. IJCAI 2019. [[paper]](https://arxiv.org/pdf/1906.04362.pdf)|
| DIM                      |   78.7  |   89.0  |   97.1  | Dually Interactive Matching Network for Personalized Response Selection in Retrieval-Based Chatbots. EMNLP 2019. [[paper]](https://www.aclweb.org/anthology/D19-1193.pdf) [[code]](https://github.com/JasonForJoy/DIM)|
| CSN                      |   69.8  |   82.7  |   94.0  | Content Selection Network for Document-grounded Retrieval-based Chatbots. ECIR 2021. [[paper]](https://arxiv.org/pdf/2101.08426.pdf) [[code]](https://github.com/DaoD/CSN)|
| RSM-DCK                  |   79.3  |   88.8  |   96.7  | Learning to Detect Relevant Contexts and Knowledge for Response Selection in Retrieval-based Dialogue Systems. CIKM 2020. [[paper]](https://dl.acm.org/doi/pdf/10.1145/3340531.3411967)|
| FIRE                     |   81.8  |   90.8  |   97.4  | Filtering before Iteratively Referring for Knowledge-Grounded Response Selection in Retrieval-Based Chatbots. EMNLP 2020: Findings. [[paper]](https://www.aclweb.org/anthology/2020.findings-emnlp.127.pdf) [[code]](https://github.com/JasonForJoy/FIRE)|

## Remark

The studies we present here may be incomplete. Please feel free to open issues, pull requests, or contact us to add more new studies.
