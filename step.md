# Smallstep CA

### Verwendung Smallstep step-ca mit `step` Command

`step` ist ein benutzerfreundliches Kommandozeilentool zum Betreiben und Automatisieren von Public Key Infrastructure (PKI)-Systemen und Arbeitsabläufen. `step` fungiert als Front-End-Schnittstelle (Client) für `step-ca`.

#### Installation `step` Command auf Windows

	winget install Smallstep.step

#### Initiale Konfiguration `step` Client Umgebung

```shell
step ca bootstrap \
  --ca-url https://pki.poly-clip.com \
  --fingerprint 480ecf4b7dcf00d22d9e84f85248e7158b1380d1d70da727a518f4287ebce72a
```

#### Root CA Zertifikat herunterladen

```shell
step ca root root_ca.crt
```

#### Signieren eines Certificate Signing Requests (CSR)

```shell
step ca sign host.domain.csr host.domain.crt
```

#### Referenzen

[Installation Client auf Windows](https://smallstep.com/docs/step-cli/installation/#windows)

[Konfiguration Client Umgebung](https://smallstep.com/docs/step-ca/getting-started/#access-your-certificate-authority)
