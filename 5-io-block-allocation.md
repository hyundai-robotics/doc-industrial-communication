# 5. Lesen und Schreiben von industriellen Kommunikations-E/A

Dies ist die Methode zur Zuweisung von E/A-Blöcken für die Kommunikation mit der Steuerung nach Abschluss der Einstellungen für die industrielle Kommunikation.

Die industrielle Kommunikations-E/A muss dem Bereich fb0 bis fb9 zugewiesen werden, um verwendet werden zu können.

<br>

{% hint style="info" %}
\.      Informationen zu den Methoden zum Lesen/Schreiben von E/A für fb-Blöcke finden Sie im folgenden Handbuch.

\.   **\[Steuerungshandbuch: Allgemeiner Eingang]**   
\.   **\[Steuerungshandbuch: Allgemeiner Ausgang]**   
{% endhint %}

<br>

##### 1. Wählen Sie das Menü zur Zuweisung von E/A-Blöcken
   Berühren Sie das Menü **\[System > 2: Steuerungsparameter > 2: Eingangs-/Ausgangssignaleinstellungen > 6: FB-Blockzuweisung]**.

<br>

##### 2. Geben Sie den industriellen Kommunikationstyp für den gewünschten fb-Bereich an.
   Tippen Sie nach der Angabe auf die Schaltfläche **\[OK]**.

![[Abbildung 5-1]](<_assets/4-io-block-allocation/image_1.png>)


{% hint style="warning" %}
**\[Achtung]**: Bei Verwendung zusammen mit einer Embedded-SPS überprüfen Sie bitte die E/A-Attribute DI/DO - X/Y. 
{% endhint %}

{% hint style="warning" %}
**\[Achtung]**: Für den EtherNet/IP-Adapter beträgt die maximale Blockgröße 120 Byte, und es können bis zu 2 ausgewählt werden. Eine Auswahl von mehr als 2 wird ignoriert. 
{% endhint %}
