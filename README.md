## Alex Freidah

Infrastructure & Platform Engineering · [alexfreidah.com](https://alexfreidah.com) 

---

### Homelab (munchbox - named after my dog Munch) and projects that spun out of it

<table>
<tr>
<td width="120" align="center">
<a href="https://github.com/afreidah/munchbox">
<img src="https://raw.githubusercontent.com/afreidah/munchbox/main/munchbox.png" width="100" alt="munchbox">
</a>
</td>
<td>
<strong><a href="https://github.com/afreidah/munchbox">munchbox</a></strong><br>
The homelab that spawned the other projects. A hybrid cloud infrastructure platform running Nomad, Consul, and Vault across local bare-metal nodes, proxmox vms, and free-tier Oracle Cloud VMs, connected over WireGuard. Always a work in progress.
</td>
</tr>
<tr>
<td width="120" align="center">
<a href="https://s3-orchestrator.munchbox.cc">
<img src="https://raw.githubusercontent.com/afreidah/s3-orchestrator/main/docs/images/logo.png" width="100" alt="s3-orchestrator">
</a>
</td>
<td>
<strong><a href="https://s3-orchestrator.munchbox.cc">s3-orchestrator</a></strong><br>
Unified S3-compatible storage across multiple backends. Stack allocations from multiple providers into a single endpoint with optional per-backend bytes and montly api/ingress/egress quota enforcement, cross-backend replication/failover, and envelope encryption.  Combine multiple free-tier accounts and tune each to avoid incurring costs and present a unified s3-endpoint to your applications/clients without any code changes required.
</td>
</tr>
<tr>
<td width="120" align="center">
<a href="https://cloudflare-log-collector.munchbox.cc">
<img src="https://raw.githubusercontent.com/afreidah/cloudflare-log-collector/main/web/static/images/logo.png" width="100" alt="cloudflare-log-collector">
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
<tr>
<td width="120" align="center">
<a href="https://nomad-temporal-jobs.munchbox.cc">
<img src="https://raw.githubusercontent.com/afreidah/nomad-temporal-jobs/main/web/static/images/logo.png" width="100" alt="nomad-temporal-jobs">
</a>
</td>
<td>
<strong><a href="https://nomad-temporal-jobs.munchbox.cc">nomad-temporal-jobs</a></strong><br>
Temporal workflow workers that automate infrastructure ops on a Nomad/Consul cluster: backups to S3, Trivy vulnerability scanning, orphaned-data cleanup, and saga-based Docker registry GC — fully traced with OpenTelemetry. 
</td>
</tr>
<tr>
<td width="120" align="center">
<a href="https://g3.munchbox.cc">
<img src="https://raw.githubusercontent.com/afreidah/g3/main/docs/logo.png" width="100" alt="g3">
</a>
</td>
<td>
<strong><a href="https://g3.munchbox.cc">g3</a></strong><br>
S3-compatible HTTP gateway that uses Gmail/Gdrive as the storage backend. Objects are stored as emails — metadata in the body, data as attachments, path as subject, and buckets as labels. Designed for write-once/read-rarely workloads like offsite backups, turning Gmail's 15 GB of free storage into a durable, API-accessible backup target.
</td>
</tr>
</table>
