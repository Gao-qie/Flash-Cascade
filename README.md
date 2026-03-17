# Flash-Cascade

># Using Multimodal Large Language Models for False Alarm Reduction in Image-based Fire Detection
https://doi.org/10.21203/rs.3.rs-8847038/v1

Existing vision-based methods suffer from high false alarm rates in urban flame detection. Applying Multimodal Large Language Models (MLLMs) for secondary filtering shows great potential in reducing false alarms, yet they have high inference latency and are prone to reasoning collapse on negative samples without explicit Chain-of-Thought (CoT) guidance. To overcome these challenges, this study proposed Flash-Cascade, the first sub-second MLLM-based firewall to leverage CoT to efficiently filter false alarms. We deconstructed the flame detection process into four logical stages (planning, observation, analysis, and judgment), which informed the design of three switchable reasoning modes (Detailed, Quick, and Rapid) to achieve inference acceleration via CoT compression. We fine-tuned Qwen2-VL-7B-Instruct on a multi-grained instruction dataset via Low-Rank Adaptation. This process internalizes explicit reasoning logic into implicit parameter representations, enabling the model to maintain robust reasoning capability even without explicit CoT guidance. On our newly constructed benchmark incorporating real-world hard negatives, Flash-Cascade achieves an accuracy of 97.79% and an F1-score of 0.9767 in Rapid mode, outperforming the baseline by 61.63 percentage points (pp) and 0.5152, respectively. Furthermore, it outperforms the state-of-the-art object detector DEIMv2 by 14.64 pp in accuracy. The method exhibits exceptional sample efficiency, converging with only 600 samples and 2 epochs, and improves inference speed by 810% over standard CoT. This study will open a door for robust and efficient flame detection in high-interference scenarios.


![图片](https://cdn-uploads.huggingface.co/production/uploads/660668f93c37e535dea3ba54/dvgZ32M2KFDWZaEE1lgdr.png)

![图片](https://cdn-uploads.huggingface.co/production/uploads/660668f93c37e535dea3ba54/vHLPZ3t3ABXWDBTqpcTnx.png)

## Weight, Installation and Simple Inference Example 
- (DeepSeekVL-1.3B-Chat-fire)[https://huggingface.co/gaoqie/DeepSeekVL-1.3B-Chat-fire]
- (DeepSeekVL-7B-Chat-fire)[https://huggingface.co/gaoqie/DeepSeekVL-7B-Chat-fire]
- (DeepSeekVL2-Tiny-fire)[https://huggingface.co/gaoqie/DeepSeekVL2-Tiny-fire]
- (Qwen2VL-2B-Instruct-fire)[https://huggingface.co/gaoqie/Qwen2VL-2B-Instruct-fire]
- (qwen2-vl-7b-instruct-fire)[https://huggingface.co/gaoqie/qwen2-vl-7b-instruct-fire]
- (Qwen2.5VL-3B-Instruct-fire)[https://huggingface.co/gaoqie/Qwen2.5VL-3B-Instruct-fire]
- (Qwen2.5VL-7B-Instruct-fire)[https://huggingface.co/gaoqie/Qwen2.5VL-7B-Instruct-fire]
- (InternVl2-8B-fire)[https://huggingface.co/gaoqie/InternVl2-8B-fire]
- (Glm-Edge-V-5B-fire)[https://huggingface.co/gaoqie/Glm-Edge-V-5B-fire]
