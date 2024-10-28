# What Happens during a DDOS Attack
## This mermaid dagram was created to show what happens during a **DDOS** attack and why **Firewalls** are a necessity.
```mermaid
sequenceDiagram
  participant Attacker
  participant botNet
  participant webSever
  participant Firewall
  Attacker->>botNet: accumulates an army of bots through infecting other PCs
  botNet->>webSever: the botnet finds the websever asigned by the attacker and sends an overwhelming amount of requests to the websever to cause it to crash
  Firewall->>botNet: receives the requests from the botnet and redistributes them to different networks to avoid crashing the websever
