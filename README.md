## Alex Freidah

Infrastructure & Platform Engineering · [website](https://alexfreidah.com) 

---

### Homelab (munchbox - named after my dog Munch) and projects that spun out of it

<table>
<tr>
<td width="80" align="center"><a href="https://github.com/afreidah/munchbox"><img src="munchbox.png" width="66" alt="munchbox"></a></td>
<td><strong><a href="https://github.com/afreidah/munchbox">munchbox</a></strong><br>Hybrid-cloud homelab running Nomad, Consul, and Vault across bare metal, Proxmox VMs, and Oracle Cloud free-tier nodes linked over WireGuard. The other projects spun out of it.</td>
</tr>
<tr>
<td width="80" align="center"><a href="https://s3-orchestrator.munchbox.cc"><img src="s3-orchestrator.png" width="52" alt="s3-orchestrator"></a></td>
<td><blockquote><strong><a href="https://github.com/afreidah/s3-orchestrator">s3-orchestrator</a></strong><br>Presents many S3-compatible providers as one S3 endpoint, with replicated copies, read failover, per-backend limits, compression, and envelope encryption.<br><br><strong>Looking for more users and contributors.</strong></blockquote></td>
</tr>
<tr>
<td width="80" align="center"><a href="https://g3.munchbox.cc"><img src="g3.png" width="80" alt="g3"></a></td>
<td><strong><a href="https://github.com/afreidah/g3">g3</a></strong><br>S3-compatible gateway backed by a Google account: object data streams to Drive with no size ceiling, Gmail messages hold the metadata, and a local SQLite index keeps metadata reads off the API entirely.</td>
</tr>
<tr>
<td width="80" align="center"><a href="https://nomad-temporal-jobs.munchbox.cc"><img src="nomad-temporal-jobs.png" width="76" alt="nomad-temporal-jobs"></a></td>
<td><strong><a href="https://github.com/afreidah/nomad-temporal-jobs">nomad-temporal-jobs</a></strong><br>Seven Temporal workers running ten scheduled jobs against the cluster: on-demand CI runners that exist only while a job is queued, Raft snapshots, image scanning, ACME and GitHub token renewal, and storage reclamation, all traced with OpenTelemetry.</td>
</tr>
<tr>
<td width="80" align="center"><a href="https://github.com/afreidah/munchbox-hashi-upgrade"><img src="munchbox-hashi-upgrade.png" width="66" alt="munchbox-hashi-upgrade"></a></td>
<td><strong><a href="https://github.com/afreidah/munchbox-hashi-upgrade">munchbox-hashi-upgrade</a></strong><br>Resumable rolling upgrades for Nomad, Consul, and Vault, with task order and health gates based on dynamically discovered cluster topology. Used to upgrade Munchbox live: Nomad over 12 hosts, Consul over 17, Vault over 3.</td>
</tr>
<tr>
<td width="80" align="center"><a href="https://cloudflare-log-collector.munchbox.cc"><img src="cloudflare-log-collector.png" width="80" alt="cloudflare-log-collector"></a></td>
<td><strong><a href="https://github.com/afreidah/cloudflare-log-collector">cloudflare-log-collector</a></strong><br>Polls Cloudflare for firewall events, HTTP traffic, account audit logs, and real browser Core Web Vitals, shipping them to Loki and Prometheus with every cycle traced to Tempo.</td>
</tr>
<tr>
<td width="80" align="center"><a href="https://oracle-watchdog.munchbox.cc"><img src="oracle-watchdog.png" width="60" alt="oracle-watchdog"></a></td>
<td><strong><a href="https://github.com/afreidah/oracle-watchdog">oracle-watchdog</a></strong><br>Auto-recovers stuck Oracle Cloud free-tier instances by watching Consul session heartbeats and driving OCI stop/start cycles.</td>
</tr>
</table>
