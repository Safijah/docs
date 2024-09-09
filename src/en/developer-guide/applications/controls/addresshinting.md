---
Author: Safija Hubljar
---

# Address Hinting

This control will hint companies based on the selected country. When the user selects one of the hinted companies, all other fields will be pre-filled. Additionally, the control allows the user to manually create a company if manual input is enabled.

![Address Hinting Displayed On Form](/.attachments/applications/Controls/addresshintingcontrol.png)

## Bindings

<table>
  <thead>
    <tr>
      <th>Property Name</th>
      <th>Description</th>
      <th>Of Type</th>
      <th>Input</th>
      <th>Output</th>
      <th>Usage</th>
      <th>Required</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>fullAddress</td>
      <td>Full address attribute to be bounded to.</td>
      <td>
      <p><code>SingleLine.Text</code></p>
      <td><p style="width: 180px"><code>Czerninská 1, 54226 Horní Maršov</code></p>
      <p><code>''</code></p>      </td>
      <td><p style="width: 180px"><code>Czerninská 1, 54226 Horní Maršov</code></p></td>
      <td><code>bound</code></td>
      <td><code>true</code></td>
    </tr>
    <tr>
      <td>addressLanguage</td>
      <td>Language in which the address should be returned.</td>
      <td><code>Enum</code></td>
      <td>
      <p><code>user-default</code></p>
      <p><code>en</code></p>
      </td>
      <td>N/A</td>
      <td><code>input</code></td>
      <td><code>true</code></td>
    </tr>
    <tr>
      <td>addressId</td>
      <td>Address id from the service.</td>
      <td><code>SingleLine.Text</code></td>
      <td>2331888</td>
      <td><code>2331888</code></td>
      <td><code>bound</code></td>
      <td><code>false</code></td>
    </tr>
    <tr>
    <td>country</td>
    <td>Country of the address.</td>
    <td><code>SingleLine.Text</code></td>
    <td>
    <p><code>Česká republika</code></p>
    </td>
    <td><p><code>Česká republika</code></p></td>
    <td><code>bound</code></td>
    <td><code>false</code></td>
  </tr>
   <tr>
    <td>countryIsoAlpha2Code</td>
    <td>Alpha 2 country ISO code of the address.</td>
    <td><code>SingleLine.Text</code></td>
    <td>
    </td>
    <td><p><code>CZ</code></p></td>
    <td><code>bound</code></td>
    <td><code>false</code></td>
  </tr>
    <tr>
      <td>administrativeArea</td>
      <td>Addministrative area of the address.</td>
      <td><code>SingleLine.Text</code></td>
      <td>
      <p><code>Královéhradecký kraj</code></p>
      </td>
      <td>
      <p><code>Královéhradecký kraj</code></p>
      </td>
      <td><code>bound</code></td>
      <td><code>false</code></td>
    </tr>
    <tr>
      <td>locality</td>
      <td>Locality of the address.</td>
      <td><code>SingleLine.Text</code></td>
      <td>
      <p><code>Svoboda nad Úpou</code></p>
      </td>
      <td>
      <p><code>Horní Maršov</code></p>
      </td>
      <td><code>bound</code></td>
      <td><code>false</code></td>
    </tr>
    <tr>
      <td>subLocality</td>
      <td>Sub-locality of the address.</td>
      <td><code>SingleLine.Text</code></td>
      <td>
      <p><code>Horní Maršov</code></p>
      </td>
      <td>
      <p><code>Horní Maršov</code></p>
      <p><code>''</code></p>
      </td>
      <td><code>bound</code></td>
      <td><code>false</code></td>
    </tr>
    <tr>
      <td>street</td>
      <td>Street of the address.</td>
      <td><code>SingleLine.Text</code></td>
      <td>
      <p><code>Czerninská</code></p>
      </td>
      <td><p><code>Czerninská</code></p></td>
      <td><code>bound</code></td>
      <td><code>false</code></td>
    </tr>
    <tr>
      <td>streetNumber</td>
      <td>Region of the company.</td>
      <td><code>SingleLine.Text</code></td>
      <td><p><code>1</code></p></td>
      <td><p><code>1</code></p></td>
      <td><code>bound</code></td>
      <td><code>false</code></td>
    </tr>
    <tr>
      <td>formattedPostalCode</td>
      <td>Formatted postal code of the address.</td>
      <td><code>SingleLine.Text</code></td>
      <td>
      <p><code>542 26</code></p>
       </td>
      <td><p><code>542 26</code></p></td>
      <td><code>bound</code></td>
      <td><code>false</code></td>
    </tr>
    <tr>
      <td>latitude</td>
      <td>Latitude (coordinates) of the address.</td>
      <td><code>Decimal</code></td>
      <td><p><code>50.66213925553594</code></p></td>
      <td><p><code>50.66213925553594</code></p></td>
      <td><code>bound</code></td>
      <td><code>false</code></td>
    </tr>
    <tr>
      <td>longitude</td>
      <td>Longitude (coordinates) of the address.</td>
      <td><code>Decimal</code></td>
      <td>
      <p><code>15.818599712569972</code></p>
      </td>
      <td><p><code>15.818599712569972</code></p></td>
      <td><code>bound</code></td>
      <td><code>false</code></td>
    </tr>
    <tr>
      <td>plusCode</td>
      <td>Open location code (OLC).</td>
      <td><p><code>SingleLine.Text</code></p>
      </td>
      <td>
      <p><code>null</code></p>
       </td>
      <td>
      <p><code>null</code></p></td>
      <td><code>bound</code></td>
      <td><code>false</code></td>
    </tr>
  <tr>
      <td>manualInput</td>
      <td>If the control is in manual mode, autocomplete is not working and the control is in read-only mode.</td>
      <td><p><code>TwoOptions</code></p>
      </td>
      <td>
      <p><code>false</code></p>
       <p><code>true</code></p>
       </td>
      <td><p><code>false</code></p></td>
      <td><code>bound</code></td>
      <td><code>false</code></td>
   </tr>
  <tr>
      <td>rawAddressJSON</td>
      <td>Raw address JSON output.</td>
      <td><p><code>SingleLine.Text</code></p>
      </td>
      <td>
       </td>
      <td>
      <p><code>{
  "country": "Česká republika",
  "countryCode": "CZ",
  "administrativeArea": "Královéhradecký kraj",
  "locality": "Svoboda nad Úpou",
  "subLocality": "Horní Maršov",
  "street": "Czerninská",
  "streetNumber": "1",
  "postalCode": "54226",
  "formattedPostalCode": "542 26",
  "latitude": 50.66213925553594,
  "longitude": 15.818599712569972,
  "text": "Czerninská 1, 54226 Horní Maršov",
  "plusCode": null,
  "administrativeAreas": [
    {
      "key": 10,
      "value": {
        "id": "643483",
        "name": "Horní Maršov",
        "source": "RUIAN"
      }
    }
  ],
  "virtualAttributes": [],
  "id": "2331888"
}
</code></p></td>
      <td><code>bound</code></td>
      <td><code>false</code></td>
   </tr>
     <tr>
      <td>geospatialExpandQuery</td>
      <td>Expand query which should be passed to geospatial Data Feed request.</td>
      <td><p><code>SingleLine.Text</code></p>
      </td>
      <td>
      <p><code>geometry($select=type,coordinates),spatialReference,boundaries($select=name,area)</code></p>
       </td>
      <td><p><code>Sokolovská 352/215, Vysočany, 19000 Praha 9</code></p>
      <p><code>''</code></p></td>
      <td><code>input</code></td>
      <td><code>false</code></td>
   </tr>
  </tbody>
</table>

## Changelog

 <h2>2024-09-02</h2>
 <h3> Changed</h3>
<ul>
  <li>Changed PCF to use latest shared component</li>
</ul>