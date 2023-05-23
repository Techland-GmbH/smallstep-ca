# Smallstep CA

### Verwendung Smallstep step-ca mit `step` Command

`step` ist ein benutzerfreundliches Kommandozeilentool zum Betreiben und Automatisieren von Public Key Infrastructure (PKI)-Systemen und Arbeitsabläufen. `step` fungiert als Front-End-Schnittstelle (Client) für `step-ca`.

#### Installation `step` Command auf Windows

	winget install Smallstep.step

#### Initiale Konfiguration `step` Client Umgebung

	step ca bootstrap --ca-url https://pki.poly-clip.com --fingerprint 0c361bafedf44bd2475a52864dc578e0c4918d556e655d9b095714a0523de4c7


#### Referenzen

[Installation Client auf Windows](https://smallstep.com/docs/step-cli/installation/#windows)
[Konfiguration Client Umgebung](https://smallstep.com/docs/step-ca/getting-started/#access-your-certificate-authority)
