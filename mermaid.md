```mermaid
sequenceDiagram
  participant Attacker
  participant botNet
  participant webSever
  participant Firewall
  Attacker->>botNet: accumulates an army of bots through other infected PCs
  botNet->>webSever: finds the websever asigned by the attacker and sends an overwhelming amount of requests to the websever to cause it to crash
  Firewall->>botNet: receives the requests from the botnet and redistributes them to different networks to avoid crashing the websever
