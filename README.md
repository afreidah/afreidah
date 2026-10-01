## Alex Freidah

Infrastructure & Platform Engineering · [website](https://alexfreidah.com) 

---

### Homelab (munchbox - named after my dog Munch) and projects that spun out of it

<table>
<tr>
<td width="120" align="center">
<a href="https://github.com/afreidah/munchbox">
<img src="munchbox.png" width="100" alt="munchbox">
</a>
</td>
<td>
<strong><a href="https://github.com/afreidah/munchbox">munchbox</a></strong><br>
The homelab that spawned the other projects. A hybrid cloud infrastructure platform running Nomad, Consul, and Vault across local bare-metal nodes, proxmox vms, and free-tier Oracle Cloud VMs, connected over WireGuard. Always a work in progress.
<br><a href="https://github.com/afreidah/munchbox/tree/main/nomad/jobs"><img src="https://img.shields.io/badge/Nomad-00CA8E?logo=nomad&logoColor=white" alt="Nomad"></a> <a href="https://github.com/afreidah/munchbox/tree/main/infrastructure/cinc/cookbooks/consul"><img src="https://img.shields.io/badge/Consul-E03875?logo=consul&logoColor=white" alt="Consul"></a> <a href="https://github.com/afreidah/munchbox/tree/main/infrastructure/cinc/cookbooks/vault"><img src="https://img.shields.io/badge/Vault-FFD814?logo=vault&logoColor=black" alt="Vault"></a> <a href="https://github.com/afreidah/munchbox/tree/main/infrastructure/cinc/cookbooks"><img src="https://img.shields.io/badge/Cinc%2FChef-F09820?logo=chef&logoColor=white" alt="Cinc/Chef"></a> <a href="https://github.com/afreidah/munchbox/tree/main/infrastructure/terragrunt/modules"><img src="https://img.shields.io/badge/Terraform-844FBA?logo=terraform&logoColor=white" alt="Terraform"></a> <a href="https://github.com/afreidah/munchbox/tree/main/infrastructure/terragrunt"><img src="https://img.shields.io/badge/Terragrunt-5C4EE5" alt="Terragrunt"></a>
</td>
</tr>
<tr>
<td width="120" align="center">
<a href="https://s3-orchestrator.munchbox.cc">
<img src="s3-orchestrator.png" width="100" alt="s3-orchestrator">
</a>
</td>
<td>
<strong><a href="https://s3-orchestrator.munchbox.cc">s3-orchestrator</a></strong><br>
Unified S3-compatible storage across multiple backends. Stack allocations from multiple providers into a single endpoint with optional per-backend bytes and montly api/ingress/egress quota enforcement, cross-backend replication/failover, and envelope encryption.  Combine multiple free-tier accounts and tune each to avoid incurring costs and present a unified s3-endpoint to your applications/clients without any code changes required.
<br><a href="https://github.com/afreidah/s3-orchestrator"><img src="https://img.shields.io/badge/mature-looking%20for%20users%20%26%20contributors-16a34a" alt="mature, looking for users and contributors"></a>
</td>
</tr>
<tr>
<td width="120" align="center">
<a href="https://nomad-temporal-jobs.munchbox.cc">
<img src="nomad-temporal-jobs.png" width="120" alt="nomad-temporal-jobs">
</a>
</td>
<td>
<strong><a href="https://nomad-temporal-jobs.munchbox.cc">nomad-temporal-jobs</a></strong><br>
Temporal workflow workers that automate infrastructure ops on a Nomad/Consul cluster: backups to S3, Trivy vulnerability scanning, orphaned-data cleanup, and saga-based Docker registry GC — fully traced with OpenTelemetry. 
</td>
</tr>
<tr>
<td width="120" align="center">
<a href="https://vagabond.munchbox.cc">
<img src="vagabond.png" width="90" alt="vagabond">
</a>
</td>
<td>
<strong><a href="https://vagabond.munchbox.cc">vagabond</a></strong><br>
Compute broker for short-lived, stateless workloads. Jobs are described once in Nomad-style HCL, and Vagabond picks the backend that can and should run them, runs them there, and reports the result. Backends are provider plugins: Google Cloud Run Jobs and AWS Lambda so far, plus your own machines running the lightweight Vagabond agent, which runs workloads as containers or Firecracker microVMs. <br><img src="https://img.shields.io/badge/early%20prototype-still%20taking%20shape-f97316" alt="early prototype, still taking shape">
</td>
</tr>
<tr>
<td width="120" align="center">
<a href="https://g3.munchbox.cc">
<img src="g3.png" width="120" alt="g3">
</a>
</td>
<td>
<strong><a href="https://g3.munchbox.cc">g3</a></strong><br>
S3-compatible HTTP gateway that uses Gmail/Gdrive as the storage backend. Objects are stored as emails — metadata in the body, data as attachments, path as subject, and buckets as labels. Designed for write-once/read-rarely workloads like offsite backups, turning Gmail's 15 GB of free storage into a durable, API-accessible backup target.
</td>
</tr>
<tr>
<td width="120" align="center">
<a href="https://cloudflare-log-collector.munchbox.cc">
<img src="cloudflare-log-collector.png" width="120" alt="cloudflare-log-collector">
</a>
</td>
<td>
<strong><a href="https://cloudflare-log-collector.munchbox.cc">cloudflare-log-collector</a></strong><br>
Cloudflare analytics collector for self-hosted observability stacks. Polls the GraphQL API for firewall events and HTTP traffic stats, ships them to Loki and Prometheus with OpenTelemetry tracing.
</td>
</tr>
<tr>
<td width="120" align="center">
<a href="https://oracle-watchdog.munchbox.cc">
<img src="https://raw.githubusercontent.com/afreidah/oracle-watchdog/main/web/static/images/logo.png" width="100" alt="oracle-watchdog">
</a>
</td>
<td>
<strong><a href="https://oracle-watchdog.munchbox.cc">oracle-watchdog</a></strong><br>
Dual monitor/agent binary. Auto-recovers stuck Oracle Cloud free-tier instances by polling Consul KV for missing session heartbeats and driving OCI stop/start cycles. Ships an optional WireGuard endpoint resolver and Cloudflare DDNS updater. </td>
</tr>
</table>
