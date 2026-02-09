### 2.4.4 Error Codes

<br>

{% hint style="info" %}
   - Provides a real-time diagnostic function by displaying the communication status of each device using CIP standard General Status codes.
{% endhint %}

<br>

![[figure 2.4.4-1 Scanner Settings]](<../../_assets/2-ethernet-ip/4-scanner/img_8.png>) 

<br>

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**General Status Codes**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Status Value (Hex)</th>
		<th class='powderblued'>Name</th>
		<th class='powderblued'>Description</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>-</td>
		<td>Communication not configured or changed</td>
		<td>Communication settings have not been applied or are in the process of changing</td>
	</tr>
	<tr>
		<td>0x00</td>
		<td>Success</td>
		<td>The service has successfully been performed by the specified
object.</td>
	</tr>
	<tr>
		<td>0x00 (In case of error)</td>
		<td>No reponse</td>
		<td>No communication response (e.g., cable disconnected, invalid IP address, etc.)</td>
	</tr>
	<tr>
		<td>0x01</td>
		<td>Connection failed</td>
		<td>A connection-elated service failed. This happened at any
location along the connection path.</td>
	</tr>
	<tr>
		<td>0x02</td>
		<td>Resource unavailable</td>
		<td>Some resources which were required for the object to perform
the requested service were not available.</td>
	</tr>
	<tr>
		<td>0x03</td>
		<td>Invalid parameter value</td>
		<td>See status code 0x20, which is usually applied in this situation.</td>
	</tr>
	<tr>
		<td>0x04</td>
		<td>Path segment error</td>
		<td>A path segment error has been encountered. Evaluation of the
supplied path information failed.</td>
	</tr>
	<tr>
		<td>0x05</td>
		<td>Path destination unknown</td>
		<td>The path references an unknown object class, instance or
structure element causing the abort of path processing.</td>
	</tr>
	<tr>
		<td>0x06</td>
		<td>Partial transfer</td>
		<td>Only a part of the expected data could be transferred.</td>
	</tr>
	<tr>
		<td>0x07</td>
		<td>Connection lost</td>
		<td>The connection for messaging has been lost.</td>
	</tr>
	<tr>
		<td>0x08</td>
		<td>Service not supported</td>
		<td>The requested service has not been implemented or has not
been defined for this object class or instance</td>
	</tr>
	<tr>
		<td>0x09</td>
		<td>Invalid attribute value</td>
		<td>Detection of invalid attribute data</td>
	</tr>
	<tr>
		<td>0x0A</td>
		<td>Attribute list error</td>
		<td>An attribute in the Get_Attribute_List or Set_Attribute_List
response has a status not equal to 0.</td>
	</tr>
	<tr>
		<td>0x0B</td>
		<td>Already in requested state</td>
		<td>The object is already in the mode or state which has been
requested by the service</td>
	</tr>
	<tr>
		<td>0x0C</td>
		<td>Object state conflict</td>
		<td>The object is not able to perform the requested service in the
current mode or state</td>
	</tr>
	<tr>
		<td>0x0D</td>
		<td>Object already exists</td>
		<td>It has been tried to create an instance of an object which
already exists.</td>
	</tr>
	<tr>
		<td>0x0E</td>
		<td>Attribute not settable</td>
		<td>It has been tried to change a non-modifiable attribute.</td>
	</tr>
	<tr>
		<td>0x0F</td>
		<td>Privilege violation</td>
		<td>A check of permissions or privileges failed</td>
	</tr>
	<tr>
		<td>0x10</td>
		<td>Device state conflict</td>
		<td>The current mode or state of the device prevents the execution
of the requested service.</td>
	</tr>
	<tr>
		<td>0x11</td>
		<td>Reply data too large</td>
		<td>The data to be transmitted in the response buffer requires more
space than the size of the allocated response buffer</td>
	</tr>
	<tr>
		<td>0x12</td>
		<td>Fragmentation of primitive value</td>
		<td>The service specified an operation that is going to fragment a
primitive data value, i.e. half a REAL data type.</td>
	</tr>
	<tr>
		<td>0x13</td>
		<td>Not enough data</td>
		<td>The service did not supply all required data to perform the
specified operation</td>
	</tr>
	<tr>
		<td>0x14</td>
		<td>Attribute not supported</td>
		<td>An unsupported attribute has been specified in the request</td>
	</tr>
	<tr>
		<td>0x15</td>
		<td>Too much data</td>
		<td>More data than was expected were supplied by the service.</td>
	</tr>
	<tr>
		<td>0x16</td>
		<td>Object does not exist</td>
		<td>The specified object does not exist in the device.</td>
	</tr>
	<tr>
		<td>0x17</td>
		<td>Service fragmentation sequence erroruccess</td>
		<td>Fragmentation sequence for this service is not currently active
for this data</td>
	</tr>
	<tr>
		<td>0x18</td>
		<td>No stored attribute data</td>
		<td>The attribute data of this object has not been saved prior to the
requested service.</td>
	</tr>
	<tr>
		<td>0x19</td>
		<td>Store operation failure</td>
		<td>The attribute data of this object could not be saved due to a
failure during the storage attempt</td>
	</tr>
	<tr>
		<td>0x1A</td>
		<td>Routing failure, request packet too large</td>
		<td>The service request packet was too large for transmission on a
network in the path to the destination. The routing device was
forced to abort the service</td>
	</tr>
	<tr>
		<td>0x1B</td>
		<td>Routing failure, response packet too large</td>
		<td>The service response packet was too large for transmission on
a network in the path from the destination. The routing device
was forced to abort the service</td>
	</tr>
	<tr>
		<td>0x1C</td>
		<td>Missing attribute list entry data</td>
		<td>The service did not supply an attribute in a list of attributes that
was needed by the service to perform the requested behavior</td>
	</tr>
	<tr>
		<td>0x1D</td>
		<td>Invalid attribute value list</td>
		<td>The service returns the list of attributes containing status
information for invalid attributes</td>
	</tr>
	<tr>
		<td>0x1E</td>
		<td>Embedded service error</td>
		<td>An embedded service caused an error</td>
	</tr>
	<tr>
		<td>0x1F</td>
		<td>Vendor specific error</td>
		<td>A vendor specific error has occurred. This error should only
occur when none of the other general error codes can correctly
be applied</td>
	</tr>
	<tr>
		<td>0x20</td>
		<td>Invalid parameter</td>
		<td>A parameter which was associated with the request was invalid.
The parameter does not meet the requirements of the CIP
specification and/or the requirements defined in the specification
of an application object.</td>
	</tr>
	<tr>
		<td>0x21</td>
		<td>Write-once value already written</td>
		<td>An attempt was made to write to a write-once medium for the
second time, or to modify a value that cannot be changed after
being established once</td>
	</tr>
	<tr>
		<td>0x22</td>
		<td>Invalid reply received</td>
		<td>An invalid reply is received. Possible causes can for instance be
among others a reply service code not matching the request
service code or a reply message shorter than the expectable
minimum size</td>
	</tr>
	<tr>
		<td>0x23</td>
		<td>Reserved</td>
		<td>-</td>
	</tr>
	<tr>
		<td>0x24</td>
		<td>Reserved</td>
		<td>-</td>
	</tr>
	<tr>
		<td>0x25</td>
		<td>Key failure in path</td>
		<td>The key segment (i.e. the first segment in the path) does not
match the destination module. More information about which
part of the key check failed can be derived from the object
specific status.</td>
	</tr>
	<tr>
		<td>0x26</td>
		<td>Path size invalid</td>
		<td>Path cannot be routed to an object due to lacking information or
too much routing data have been included</td>
	</tr>
	<tr>
		<td>0x27</td>
		<td>Unexpected attribute in list</td>
		<td>It has been attempted to set an attribute which may not be set in
the current situation</td>
	</tr>
	<tr>
		<td>0x28</td>
		<td>Invalid member ID</td>
		<td>The Member ID specified in the request is not available within
the specified class/ instance or attribute</td>
	</tr>
	<tr>
		<td>0x29</td>
		<td>Member cannot be set</td>
		<td>A request to modify a member which cannot be modified has
occurred</td>
	</tr>
	<tr>
		<td>0x2A</td>
		<td>Group 2 only server general failure</td>
		<td>This DeviceNet-specific error cannot occur in EtherNet/IP</td>
	</tr>
	<tr>
		<td>0x2B - 0xCF</td>
		<td>Reserved</td>
		<td>-</td>
	</tr>
	<tr>
		<td>0xD0 - 0xFF</td>
		<td>Vendor specific Codes</td>
		<td>An object class specific error has occurred</td>
	</tr>
</tbody>
</table>
<br>
