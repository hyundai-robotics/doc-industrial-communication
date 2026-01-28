#### 1.3.7.6 DeviceNet Object


<br>

**1. Objekt**


Das DeviceNet-Gerät besteht aus einer Sammlung von Objekten. Jedes Objekt repräsentiert eine bestimmte Komponente innerhalb des Geräts.

<br>

![[Abbildung 1.3.7.6-1 DeviceNet Object]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_1.png>) 


<br>

Objekte werden anhand des Klassencodes unterschieden.

<br>

![[Abbildung 1.3.7.6-2 DeviceNet Object]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_2.png>)

<br>

Objekte bestehen aus Instanznummern und Attribut-IDs.

<br>

Der DeviceNet-Master kann über explizite Meldungen auf Objekte bestimmter Slaves zugreifen.

<br>

{% hint style="info" %}
\.      Beispiel: Objekt von Crevis GN-9212 (Diese Informationen finden Sie im Crevis-Handbuch.)

\.      Lesen des Vendor-ID-Werts des Identitätsobjekts (Klassencode 0x01)

\.      Instanz: 1

\.      Attribut-ID: 1

\.      Berechtigung: Abrufen (nur Lesen möglich)
{% endhint %}


![[Abbildung 1.3.7.6-3 DeviceNet Object Crevis GN-9212]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_3.png>)


<br>

Jedes Objekt, jede Instanz und jedes Attribut im Inneren verfügt über unterschiedliche Zugriffsberechtigungen.

<br>

{% hint style="info" %}
\.      Zugriffsberechtigungen

\.      Abrufen: Leseberechtigung

\.      Festlegen: Schreibberechtigung

\.      Einzelnes Attribut: Es kann jeweils nur auf ein Attributelement zugegriffen werden.

\.      Alle Attribute: Es kann auf alle Attribute in der Instanz gleichzeitig zugegriffen werden.
{% endhint %}

<br>