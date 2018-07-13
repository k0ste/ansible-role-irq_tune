# ansible-role-irq_tune

JSON configurable manual IRQ tunning via
[irq-tune](//github.com/k0ste/irq-tune).

## Requirements

* Ansible 2.5+;

## Example configuration

```yaml
---
# Model name:            Intel(R) Xeon(R) CPU E5-2609 v4 @ 1.70GHz
# Core(s) per socket:    8
# NUMA node0 CPU(s):     0-7

irq_tune:
- irq_auto:
  - name: 'i40e-ten0-TxRx-0'
    cores: [0] # <-- 'cores' should be list!
  - name: 'i40e-ten0-TxRx-1'
    cores: [1]
  - name: 'i40e-ten0-TxRx-2'
    cores: [2]
  - name: 'i40e-ten0-TxRx-3'
    cores: [3]
  - name: 'i40e-ten0-TxRx-4'
    cores: [4]
  - name: 'i40e-ten0-TxRx-5'
    cores: [5]
  - name: 'i40e-ten0-TxRx-6'
    cores: [6]
  - name: 'i40e-ten0-TxRx-7'
    cores: [7]
  - name: 'i40e-ten1-TxRx-0'
    cores: [7]
  - name: 'i40e-ten1-TxRx-1'
    cores: [6]
  - name: 'i40e-ten1-TxRx-2'
    cores: [5]
  - name: 'i40e-ten1-TxRx-3'
    cores: [4]
  - name: 'i40e-ten1-TxRx-4'
    cores: [3]
  - name: 'i40e-ten1-TxRx-5'
    cores: [2]
  - name: 'i40e-ten1-TxRx-6'
    cores: [1]
  - name: 'i40e-ten1-TxRx-7'
    cores: [0]
  - name: 'i40e-ten2-TxRx-0'
    cores: [0]
  - name: 'i40e-ten2-TxRx-1'
    cores: [1]
  - name: 'i40e-ten2-TxRx-2'
    cores: [2]
  - name: 'i40e-ten2-TxRx-3'
    cores: [3]
  - name: 'i40e-ten2-TxRx-4'
    cores: [4]
  - name: 'i40e-ten2-TxRx-5'
    cores: [5]
  - name: 'i40e-ten2-TxRx-6'
    cores: [6]
  - name: 'i40e-ten2-TxRx-7'
    cores: [7]
  - name: 'i40e-ten3-TxRx-0'
    cores: [7]
  - name: 'i40e-ten3-TxRx-1'
    cores: [6]
  - name: 'i40e-ten3-TxRx-2'
    cores: [5]
  - name: 'i40e-ten3-TxRx-3'
    cores: [4]
  - name: 'i40e-ten3-TxRx-4'
    cores: [3]
  - name: 'i40e-ten3-TxRx-5'
    cores: [2]
  - name: 'i40e-ten3-TxRx-6'
    cores: [1]
  - name: 'i40e-ten3-TxRx-7'
    cores: [0]
- irq_static:
  - name: 'megasas'
    cores: [0]
    irq: '26'
  - name: 'megasas'
    cores: [1]
    irq: '27'
  - name: 'megasas'
    cores: [2]
    irq: '28'
  - name: 'megasas'
    cores: [3]
    irq: '29'
  - name: 'megasas'
    cores: [4]
    irq: '30'
  - name: 'megasas'
    cores: [5]
    irq: '31'
  - name: 'megasas'
    cores: [6]
    irq: '32'
  - name: 'megasas'
    cores: [7]
    irq: '33'
```
