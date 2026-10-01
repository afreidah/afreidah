## Alex Freidah

Infrastructure & Platform Engineering · [website](https://alexfreidah.com) 

---

### Homelab (munchbox - named after my dog Munch) and projects that spun out of it

<table>
<tr>
<td width="80" align="center"><a href="https://github.com/afreidah/munchbox"><img src="munchbox.png" width="66" alt="munchbox"></a></td>
<td><strong><a href="https://github.com/afreidah/munchbox">munchbox</a></strong> <a href="https://github.com/afreidah/munchbox/tree/main/nomad/jobs"><img src="https://img.shields.io/badge/Nomad-00CA8E?logo=nomad&logoColor=white" alt="Nomad"></a> <a href="https://github.com/afreidah/munchbox/tree/main/infrastructure/cinc/cookbooks/consul"><img src="https://img.shields.io/badge/Consul-E03875?logo=consul&logoColor=white" alt="Consul"></a> <a href="https://github.com/afreidah/munchbox/tree/main/infrastructure/cinc/cookbooks/vault"><img src="https://img.shields.io/badge/Vault-FFD814?logo=vault&logoColor=black" alt="Vault"></a> <a href="https://github.com/afreidah/munchbox/tree/main/infrastructure/cinc/cookbooks"><img src="https://img.shields.io/badge/Cinc%2FChef-F09820?logo=chef&logoColor=white" alt="Cinc/Chef"></a> <a href="https://github.com/afreidah/munchbox/tree/main/infrastructure/terragrunt/modules"><img src="https://img.shields.io/badge/Terraform-844FBA?logo=terraform&logoColor=white" alt="Terraform"></a> <a href="https://github.com/afreidah/munchbox/tree/main/infrastructure/terragrunt"><img src="https://img.shields.io/badge/Terragrunt-5C4EE5" alt="Terragrunt"></a><br>Hybrid-cloud homelab running Nomad, Consul, and Vault across bare metal, Proxmox VMs, and Oracle Cloud free-tier nodes linked over WireGuard. The other projects spun out of it.</td>
</tr>
<tr>
<td width="80" align="center"><a href="https://s3-orchestrator.munchbox.cc"><img src="s3-orchestrator.png" width="52" alt="s3-orchestrator"></a></td>
<td><strong><a href="https://s3-orchestrator.munchbox.cc">s3-orchestrator</a></strong> <a href="https://github.com/afreidah/s3-orchestrator"><img src="https://img.shields.io/badge/mature-looking%20for%20users%20%26%20contributors-16a34a" alt="mature, looking for users and contributors"></a><br>Presents many S3-compatible providers as one S3 endpoint, with replicated copies, read failover, per-backend limits, compression, and envelope encryption.</td>
</tr>
<tr>
<td width="80" align="center"><a href="https://vagabond.munchbox.cc"><img src="vagabond.png" width="54" alt="vagabond"></a></td>
<td><strong><a href="https://vagabond.munchbox.cc">vagabond</a></strong> <img src="https://img.shields.io/badge/early%20prototype-still%20taking%20shape-f97316" alt="early prototype, still taking shape"><br>Compute broker for short-lived workloads: describe a job once in Nomad-style HCL and it runs on Cloud Run, Lambda, or your own machines.</td>
</tr>
<tr>
<td width="80" align="center"><a href="https://nomad-temporal-jobs.munchbox.cc"><img src="nomad-temporal-jobs.png" width="76" alt="nomad-temporal-jobs"></a></td>
<td><strong><a href="https://nomad-temporal-jobs.munchbox.cc">nomad-temporal-jobs</a></strong><br>Temporal workers that automate Nomad/Consul cluster ops: S3 backups, Trivy scans, orphaned-data cleanup, and registry GC, traced with OpenTelemetry.</td>
</tr>
<tr>
<td width="80" align="center"><a href="https://g3.munchbox.cc"><img src="g3.png" width="80" alt="g3"></a></td>
<td><strong><a href="https://g3.munchbox.cc">g3</a></strong><br>S3-compatible gateway that stores objects as Gmail messages, turning 15 GB of free mail storage into an offsite backup target.</td>
</tr>
<tr>
<td width="80" align="center"><a href="https://github.com/afreidah/munchbox-hashi-upgrade"><img src="munchbox-hashi-upgrade.png" width="66" alt="munchbox-hashi-upgrade"></a></td>
<td><strong><a href="https://github.com/afreidah/munchbox-hashi-upgrade">munchbox-hashi-upgrade</a></strong><br>Resumable rolling upgrades for Nomad, Consul, and Vault, with task order and health gates derived from the cluster itself.</td>
</tr>
<tr>
<td width="80" align="center"><a href="https://cloudflare-log-collector.munchbox.cc"><img src="cloudflare-log-collector.png" width="80" alt="cloudflare-log-collector"></a></td>
<td><strong><a href="https://cloudflare-log-collector.munchbox.cc">cloudflare-log-collector</a></strong><br>Polls Cloudflare's GraphQL API for firewall events and traffic stats and ships them to Loki and Prometheus.</td>
</tr>
<tr>
<td width="80" align="center"><a href="https://oracle-watchdog.munchbox.cc"><img src="oracle-watchdog.png" width="60" alt="oracle-watchdog"></a></td>
<td><strong><a href="https://oracle-watchdog.munchbox.cc">oracle-watchdog</a></strong><br>Auto-recovers stuck Oracle Cloud free-tier instances by watching Consul session heartbeats and driving OCI stop/start cycles.</td>
</tr>
</table>
