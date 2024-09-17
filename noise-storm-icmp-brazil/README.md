Record of a large ICMP Noise Storm that appears to have an embedded message in it.

The original PCAP file has been split to accommodate GH restrictions. To stitch them back together use [`mergecap`](https://gitlab.com/wireshark/wireshark):

```bash
$ mergecap -w merged_output.pcap \
  noise-storm-icmp-brazil_00000_20240816160936.pcap \
  noise-storm-icmp-brazil_00001_20240819222104.pcap \
  noise-storm-icmp-brazil_00002_20240820165721.pcap \
  noise-storm-icmp-brazil_00003_20240821113203.pcap \
  noise-storm-icmp-brazil_00004_20240822060521.pcap \
  noise-storm-icmp-brazil_00005_20240823005218.pcap \
  noise-storm-icmp-brazil_00006_20240823192859.pcap \
  noise-storm-icmp-brazil_00007_20240824141504.pcap \
  noise-storm-icmp-brazil_00008_20240825090124.pcap \
  noise-storm-icmp-brazil_00009_20240826035404.pcap \
  noise-storm-icmp-brazil_00010_20240826231701.pcap \
  noise-storm-icmp-brazil_00011_20240827184617.pcap \
  noise-storm-icmp-brazil_00012_20240828142706.pcap \
  noise-storm-icmp-brazil_00013_20240829100324.pcap \
  noise-storm-icmp-brazil_00014_20240830052320.pcap
```