Tipos de Serviços e o que é oferecido de acordo com cada um

IaaS - infraestrutura como service
- Servidores e armazenamento
- Firewalls/segurança de rede
- Planta física/edifício do datacenter

PaaS - plataforma como serviço
- Sistemas operacionais
- Ferramentas para desenvolvedores
- Análise de negócio
- Gerenciamento de database

SaaS - software como serviço
- Aplicativos
- Apps hospedados

```mermaid
graph TD
    IaaS["IaaS - infraestrutura como serviço"]
    PaaS["PaaS - plataforma como serviço"]
    SaaS["SaaS - software como serviço"]

    IaaS --> IA1["Servidores e armazenamento"]
    IaaS --> IA2["Firewalls/segurança de rede"]
    IaaS --> IA3["Planta física/edifício do datacenter"]

    PaaS --> PA1["Sistemas operacionais"]
    PaaS --> PA2["Ferramentas para desenvolvedores"]
    PaaS --> PA3["Análise de negócio"]
    PaaS --> PA4["Gerenciamento de database"]

    SaaS --> SA1["Aplicativos"]
    SaaS --> SA2["Apps hospedados"]
```