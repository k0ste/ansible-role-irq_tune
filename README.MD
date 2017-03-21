ansible-role-irq_tune
======================

JSON configurable manual IRQ tunning via [irq-tune](//github.com/k0ste/irq-tune).

Ansible versions
------------------

Role is adapted for Ansible 2.0, should work on 1.9.

Requirements for usage
-----------------------

* GNU/Linux;
* Python2 or Python3;
* git;

Example configuration
-------------------------

```yaml
---
#Model name:            Intel(R) Xeon(R) CPU E5-2670 0 @ 2.60GHz
#Core(s) per socket:    8
#NUMA node0 CPU(s):     0-7
#NUMA node1 CPU(s):     8-15
irq_tune:
- name: 'ten0-TxRx-0'
  cores: '0'
- name: 'ten0-TxRx-1'
  cores: '1'
- name: 'ten0-TxRx-2'
  cores: '2'
- name: 'ten0-TxRx-3'
  cores: '3'
- name: 'ten0-TxRx-4'
  cores: '4'
- name: 'ten0-TxRx-5'
  cores: '5'
- name: 'ten0-TxRx-6'
  cores: '6'
- name: 'ten0-TxRx-7'
  cores: '7'
- name: 'ten1-TxRx-0'
  cores: '8'
- name: 'ten1-TxRx-1'
  cores: '9'
- name: 'ten1-TxRx-2'
  cores: '10'
- name: 'ten1-TxRx-3'
  cores: '11'
- name: 'ten1-TxRx-4'
  cores: '12'
- name: 'ten1-TxRx-5'
  cores: '13'
- name: 'ten1-TxRx-6'
  cores: '14'
- name: 'ten1-TxRx-7'
  cores: '15'
- name: 'gig2-TxRx-0'
  cores: '0'
- name: 'gig2-TxRx-1'
  cores: '1'
- name: 'gig2-TxRx-2'
  cores: '2'
- name: 'gig2-TxRx-3'
  cores: '3'
- name: 'gig2-TxRx-4'
  cores: '4'
- name: 'gig2-TxRx-5'
  cores: '5'
- name: 'gig2-TxRx-6'
  cores: '6'
- name: 'gig2-TxRx-7'
  cores: '7'
- name: 'gig3-TxRx-0'
  cores: '8'
- name: 'gig3-TxRx-1'
  cores: '9'
- name: 'gig3-TxRx-2'
  cores: '10'
- name: 'gig3-TxRx-3'
  cores: '11'
- name: 'gig3-TxRx-4'
  cores: '12'
- name: 'gig3-TxRx-5'
  cores: '13'
- name: 'gig3-TxRx-6'
  cores: '14'
- name: 'gig3-TxRx-7'
  cores: '15'
```
