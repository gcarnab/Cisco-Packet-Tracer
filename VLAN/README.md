# GCARNAB CISCO PACKET TRACER REPOSITORY >> VLAN
___

By GCARNAB <a href='https://github.com/gcarnab'> <img src='https://avatars.githubusercontent.com/u/15156604?v=4' width="50"/></a>
___

## Contents

- Cisco Packet Tracer .pkt files

## Resources

- **Prof Site** : https://sites.google.com/view/gcprof/

## Tutorial

**Definizione** :

Le VLAN, o **Virtual Local Area Network**, sono una tecnologia di rete che consente di suddividere una rete locale fisica in segmenti logici. In altre parole, le VLAN creano reti virtuali all'interno di una rete fisica, consentendo di raggruppare i dispositivi in base a criteri specifici, come reparto, funzione o sicurezza.

**Funzionamento** :

Le VLAN funzionano utilizzando identificatori speciali chiamati tag VLAN. Ogni frame di rete contiene un tag VLAN, che identifica a quale VLAN appartiene il frame. Gli switch supportati VLAN utilizzano i tag VLAN per inoltrare i frame solo alle porte appartenenti alla stessa VLAN. In questo modo, il traffico viene segmentato, riducendo la congestione e migliorando la sicurezza.

**Tipi di VLAN** :

- VLAN basate su porte: I dispositivi vengono assegnati a VLAN specifiche in base alla porta a cui sono collegati.
- VLAN basate su MAC: I dispositivi vengono assegnati a VLAN specifiche in base al loro indirizzo MAC.
- VLAN basate su protocollo: I dispositivi vengono assegnati a VLAN specifiche in base al protocollo di rete che utilizzano (ad esempio, IP o VoIP).
- VLAN dinamiche: L'assegnazione delle VLAN viene gestita automaticamente da un server, come un server RADIUS.

**Implementazione di VLAN** :

Per implementare le VLAN, è necessario uno switch supportato VLAN. Lo switch deve essere configurato per creare le VLAN desiderate e assegnare le porte e i dispositivi alle VLAN appropriate.

**Vantaggi delle VLAN** :

- Migliorata sicurezza: Le VLAN possono isolare il traffico tra diverse VLAN, limitando l'accesso non autorizzato alle risorse di rete.
- Maggiore efficienza: Le VLAN possono ridurre la congestione di rete **separando il traffico broadcast e multicast**.
- Migliore scalabilità: Le VLAN facilitano l'aggiunta di nuovi dispositivi alla rete senza dover riconfigurare l'intera rete.
- Maggiore flessibilità: Le VLAN consentono di raggruppare i dispositivi in base a criteri personalizzati, anziché solo in base alla loro posizione fisica.

**Switchport** :

Switchport mode access e trunk sono due modalità di funzionamento per le porte su uno switch di rete. La scelta della modalità dipende da come la porta verrà utilizzata per connettere dispositivi e reti.

**Porta di accesso (switchport access)**:
- Funzione: Una porta di accesso è progettata per connettere un singolo dispositivo o un segmento di rete che appartiene a una singola VLAN (Virtual Local Area Network).
- Traffico consentito: La porta consente solo il traffico associato alla VLAN assegnata. I frame Ethernet in entrata devono avere il tag VLAN corretto per essere inoltrati sulla porta. I frame Ethernet in uscita dalla porta vengono automaticamente taggati con la VLAN assegnata.
- Vantaggi:
    - Migliora la sicurezza della rete isolando il traffico tra VLAN diverse.
    - Semplifica la gestione della rete.
    - Migliora le prestazioni della rete riducendo la congestione.  

**Porta Trunk (switchport trunk)**:    
- Funzione: Una porta trunk è progettata per **trasportare il traffico di più VLAN su un singolo collegamento fisico**.
- Traffico consentito: La porta consente il traffico taggato con più VLAN. I frame Ethernet devono avere un tag VLAN valido per essere inoltrati correttamente.
- Vantaggi:
    - Riduce il numero di cavi necessari per collegare switch con più VLAN.
    - Offre maggiore scalabilità per reti con un numero elevato di VLAN.