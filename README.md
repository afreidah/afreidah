## Alex Freidah

Infrastructure & Platform Engineering · [alexfreidah.com](https://alexfreidah.com) · [Resume](https://resume.alexfreidah.com)

---

### Homelab

<a href="https://github.com/afreidah/munchbox/">
  <img src="https://img.shields.io/badge/munchbox-homelab-334155?style=for-the-badge&logo=hashicorp&logoColor=white" alt="munchbox">
</a>

A hybrid cluster spanning bare-metal nodes and free-tier cloud VMs, running Nomad, Consul, and Vault. Always has work to be done.

---

### Projects

Tools I built in Go that grew out of the homelab to solve problems I kept running into.

<table>
<tr>
<td width="120" align="center">
<a href="https://s3-orchestrator.munchbox.cc">
<img src="https://raw.githubusercontent.com/afreidah/s3-orchestrator/main/docs/images/logo.png" width="100" alt="s3-orchestrator">
</a>
</td>
<td>
<strong><a href="https://s3-orchestrator.munchbox.cc">s3-orchestrator</a></strong><br>
Unified S3-compatible storage across multiple backends. Stack free-tier allocations from multiple providers into a single endpoint with per-backend quotas, cross-backend replication, and envelope encryption.
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
Distributed monitoring and recovery for Oracle Cloud free-tier instances. Detects unresponsive nodes via Consul session heartbeats and automatically triggers OCI stop/start cycles.
</td>
</tr>
</table>
