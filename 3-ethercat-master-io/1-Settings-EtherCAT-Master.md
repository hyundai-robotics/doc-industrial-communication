## 3.1 EtherCAT-Master-E/A-Einstellungen

<br>

**1. Tippen Sie auf das Menü, um den Einstellungsbildschirm aufzurufen.**
**\[System > 2: Steuerungsparameter > 11: Industrielle Kommunikation > 4: EtherCAT-Master-Einstellungen]**

<br>

![[Abbildung 3.1-1 EtherCAT-Master-Einstellungen]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_1.png>) 

<br>

{% hint style="info" %}
   - Überprüfen Sie die ausgewählte LAN-Portnummer der Steuerung auf dem Bildschirm „EtherCAT-Master-Einstellungen“. 
{% endhint %}

**2. Verbinden Sie den LAN-Anschluss der Steuerung und die Kabel der Remote-E/A usw. für die Kommunikation und überprüfen Sie den Status.**

<br>

![[Abbildung 3.1-2 Hardware-Anschluss]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_2.png>) 
![[Abbildung 3.1-3 Hardware-Anschluss]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_3.png>) 

<br>

{% hint style="info" %}
   - Bitte verbinden Sie die Steuerung und die Remote-E/A über ein LAN-Kabel.

   - Stellen Sie alle DIP-Schalter des Remote-E/A auf AUS.

   - Schließen Sie sowohl die Remote-E/A-Stromversorgung als auch die Feldstromversorgung an. (24 V DC)
{% endhint %}

<br>

**3. Wählen Sie im Einstellungsmenü „ON“ für die Verwendung des EtherCAT-Masters.**

<br>

![[Abbildung 3.1-4 EtherCAT-Master-Einstellungen]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_4.png>) 

<br>

{% hint style="info" %}
   - Stellen Sie den Kommunikationszyklus entsprechend Ihrer Umgebung ein.

   - Es werden Kommunikationszyklen von 1 ms, 2 ms und 5 ms unterstützt.
{% endhint %}

<br>

**4. Wählen Sie im Einstellungsmenü aus der Slave-Liste die gleiche Konfiguration wie für das angeschlossene Remote-E/A-Modul aus.**

<br>

![[Abbildung 3.1-5 Crevis M9386]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_5.png>)

<br>

{% hint style="info" %}
   - Überprüfen Sie die Anzahl der Eingangs- und Ausgangs-Bytes.
{% endhint %}

<br>

{% hint style="info" %}
   - Input Module  
   - M12DF: Digital 16 Punkte
   - M3534: Analog 4 Punkte
{% endhint %}

{% hint style="info" %}
   - Ausgabemodul  
   - M225F: Digital 16 Punkte  
   - M226F: Digital 16 Punkte  
   - M2768: Digital 8 Punkte   
   - M4534: Analog 4 Punkte  
{% endhint %}

{% hint style="info" %}
   - Special Module  
   - M5112 : Conveyer I/F 
{% endhint %}

<br>

![[Abbildung 3.1-6 EtherCAT-Master-Einstellungen]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_6.png>) 

<br>

**5. Starten Sie die Steuerung nach Abschluss der Einstellungen neu.**

![[Abbildung 3.1-7 EtherCAT-Master-Einstellungen]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_7.png>) 

<br>

![[Abbildung 3.1-8 EtherCAT-Master-Einstellungen]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_8.png>) 

<br>

{% hint style="info" %}
   - Bitte starten Sie die Steuerung nach Abschluss der Einstellungen neu.
{% endhint %}

<br>

**6. Nachdem Sie sich vergewissert haben, dass die Einstellungen übernommen wurden, überprüfen Sie den Kommunikationsstatus.**

![[Abbildung 3.1-9 EtherCAT-Master-Einstellungen]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_9.png>) 

<br>

{% hint style="info" %}
   - Überprüfen Sie den Status der Kommunikationsverbindung und den Fehlerstatus.
{% endhint %}

<br>

![[Abbildung 3.1-10 Crevis M9386]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_10.png>)

<br>

{% hint style="info" %}
   - Überprüfen Sie anhand der LEDs am Remote-E/A-Modul, ob die Kommunikation ordnungsgemäß hergestellt wurde.
{% endhint %}

<br>

{% hint style="info" %}
   **Sollte ein Fehler (ERROR) im Kommunikationsstatus auftreten, beachten Sie bitte den Abschnitt („[**3.2 Fehlerbehandlung bei EtherCAT-Master-E/A**](../3-ethercat-master-io/2-Error-EtherCAT-Master.md)“).**
{% endhint %}

<br>

**7. Weisen Sie nach Abschluss der Kommunikationseinstellungen einen E/A-Block zu.**

{% hint style="info" %}
   **Nach Abschluss der Kommunikationseinstellungen können Sie Eingangs-/Ausgangssignale verwenden, indem Sie E/A-Blöcke zuweisen. Bitte beachten Sie („[**4. Zuweisung von E/A-Blöcken für die industrielle Kommunikation**](../4-io-block-allocation.md)“).**
{% endhint %}

