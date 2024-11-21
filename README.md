<h3 align="center">
    Run LLMs and AI on Any Cloud
</h3>

----
:fire: *News* :fire:
- [Sep, 2023] [**Mistral 7B**](https://mistral.ai/news/announcing-mistral-7b/), a high-quality open LLM, was released! Deploy via SkyPilot on any cloud: [**Mistral docs**](https://docs.mistral.ai/cloud-deployment/skypilot/)
- [Sep, 2023] Case study: [**Covariant**](https://covariant.ai/) transformed AI development on the cloud using SkyPilot, delivering models 4x faster cost-effectively: [**read the case study**](https://blog.skypilot.co/covariant/)
- [Aug, 2023] Cookbook: Finetuning Llama 2 in your own cloud environment, privately: [**example**](./llm/vicuna-llama-2/), [**blog post**](https://blog.skypilot.co/finetuning-llama2-operational-guide/)
- [July, 2023] Self-Hosted **Llama-2 Chatbot** on Any Cloud: [**example**](./llm/llama-2/)
- [June, 2023] Serving LLM 24x Faster On the Cloud [**with vLLM**](https://vllm.ai/) and SkyPilot: [**example**](./llm/vllm/), [**blog post**](https://blog.skypilot.co/serving-llm-24x-faster-on-the-cloud-with-vllm-and-skypilot/)
- [April, 2023] [SkyPilot YAMLs](./llm/vicuna/) for finetuning & serving the [Vicuna LLM](https://lmsys.org/blog/2023-03-30-vicuna/) with a single command!
----

SkyPilot is a framework for running LLMs, AI, and batch jobs on any cloud, offering maximum cost savings, highest GPU availability, and managed execution.

SkyPilot **abstracts away cloud infra burdens**:
- Launch jobs & clusters on any cloud
- Easy scale-out: queue and run many jobs, automatically managed
- Easy access to object stores (S3, GCS, R2)

SkyPilot **maximizes GPU availability for your jobs**:
* Provision in all zones/regions/clouds you have access to ([the _Sky_](https://arxiv.org/abs/2205.07147)), with automatic failover

SkyPilot **cuts your cloud costs**:
* [Managed Spot](https://skypilot.readthedocs.io/en/latest/examples/spot-jobs.html): 3-6x cost savings using spot VMs, with auto-recovery from preemptions
* Optimizer: 2x cost savings by auto-picking the cheapest VM/zone/region/cloud
* [Autostop](https://skypilot.readthedocs.io/en/latest/reference/auto-stop.html): hands-free cleanup of idle clusters

SkyPilot supports your existing GPU, TPU, and CPU workloads, with no code changes.

Install with pip:
```bash
pip install "skypilot[aws,gcp,azure,ibm,oci,scp,lambda,kubernetes]"  # choose your clouds
```
To get the latest features/updates, install [from source](https://skypilot.readthedocs.io/en/latest/getting-started/installation.html) or the nightly build:
```bash
pip install -U "skypilot-nightly[aws,gcp,azure,ibm,oci,scp,lambda,kubernetes]"  # choose your clouds
```

Current supported providers (AWS, Azure, GCP, Lambda Cloud, IBM, Samsung, OCI, Cloudflare, any Kubernetes cluster):
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/skypilot-org/skypilot/master/docs/source/images/cloud-logos-dark.png">
    <img alt="SkyPilot" src="https://raw.githubusercontent.com/skypilot-org/skypilot/master/docs/source/images/cloud-logos-light.png" width=80%>
  </picture>
</p>

