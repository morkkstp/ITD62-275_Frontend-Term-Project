# ITD62-275_Frontend-TermProject
Demo: https://youtu.be/buzSrQo4dlg
# อธิบายเกี่ยวกับ Term Project
- เป็น term project เกี่ยวกับระบบจองเต็นท์สำหรับพนักงาน โดยพนักงานเป็นคนกรอกข้อมูลต่างๆของนักท่องเที่ยวที่เดินเข้าไปจองเต็นท์กับพนักงาน
- พนักงานจะเปลี่ยนการกรอกข้อมูลในกระดาษเป็นกรอกข้อมูลในระบบ Website จะช่วยในการกรอกข้อมูลที่ง่ายขึ้นและสามารถดูข้อมูลทั้งหมดได้

&nbsp;&nbsp;&nbsp;&nbsp;วัตถุประสงค์ของการทำระบบจองเต็นท์สำหรับพนักงาน คือ เพื่อตอบสนองกลุ่มใช้งานของพนักงานในการให้บริการหน้าเคาน์เตอร์หรือหน่วยบริการ เพื่อจัดการให้การจองเป็นระบบมากยิ่งขึ้นและจัดเก็บข้อมูลได้ครบถ้วน อาทิ วันเริ่มจอง, วันสิ้นสุดการจอง, ข้อมูลผู้จอง ชื่อ-สกุล-เบอร์โทร-เลขบัตรประชาชน-ที่อยู่, การเช่าอุปกรณ์ที่มีให้บริการจากทางร้าน, และการบันทึกการชำระเงินและเก็บหลักฐานการชำระเงิน, นอกจากนี้ระบบยังมีความสามารถในการแก้ไขและลบข้อมูล อีกทั้งยังสามารถส่งออกข้อมูลเป็นไฟล์ Excel ได้อีกด้วย
# Data Dictionary
Data Dictionary เก็บข้อมูลทั่วไป<br>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax">#</th>
    <th class="tg-0pky">Attribute</th>
    <th class="tg-0lax">Description</th>
    <th class="tg-0lax">Data Type</th>
    <th class="tg-0lax">Example</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">1</td>
    <td class="tg-0lax">id</td>
    <td class="tg-0lax">id รายการจองเต็นท์</td>
    <td class="tg-0lax">int</td>
    <td class="tg-0lax">1</td>
  </tr>
  <tr>
    <td class="tg-0lax">2</td>
    <td class="tg-0lax">firstname</td>
    <td class="tg-0lax">ชื่อจริง</td>
    <td class="tg-0lax">string</td>
    <td class="tg-0lax">จิตราพร</td>
  </tr>
  <tr>
    <td class="tg-0lax">3</td>
    <td class="tg-0lax">lastname</td>
    <td class="tg-0lax">นามสกุล</td>
    <td class="tg-0lax">string</td>
    <td class="tg-0lax">ทองคง</td>
  </tr>
  <tr>
    <td class="tg-0lax">4</td>
    <td class="tg-0lax">phonenumber</td>
    <td class="tg-0lax">เบอร์โทรศัพท์</td>
    <td class="tg-0lax">string</td>
    <td class="tg-0lax">0857743364</td>
  </tr>
  <tr>
    <td class="tg-0lax">5</td>
    <td class="tg-0lax">idcard</td>
    <td class="tg-0lax">หมายเลขบัตรประชาชน</td>
    <td class="tg-0lax">string</td>
    <td class="tg-0lax">1849903647253</td>
  </tr>
  <tr>
    <td class="tg-0lax">6</td>
    <td class="tg-0lax">address</td>
    <td class="tg-0lax">ที่อยู่</td>
    <td class="tg-0lax">string</td>
    <td class="tg-0lax">11/55</td>
  </tr>
  <tr>
    <td class="tg-0lax">7</td>
    <td class="tg-0lax">subdistrict</td>
    <td class="tg-0lax">ตำบล</td>
    <td class="tg-0lax">string</td>
    <td class="tg-0lax">ตลาด</td>
  </tr>
  <tr>
    <td class="tg-0lax">8</td>
    <td class="tg-0lax">district</td>
    <td class="tg-0lax">อำเภอ</td>
    <td class="tg-0lax">string</td>
    <td class="tg-0lax">เมืองสุราษฎร์ธานี</td>
  </tr>
  <tr>
    <td class="tg-0lax">9</td>
    <td class="tg-0lax">province</td>
    <td class="tg-0lax">จังหวัด</td>
    <td class="tg-0lax">string</td>
    <td class="tg-0lax">สุราษฎร์ธานี</td>
  </tr>
  <tr>
    <td class="tg-0lax">10</td>
    <td class="tg-0lax">postcode</td>
    <td class="tg-0lax">รหัสไปรษณีย์</td>
    <td class="tg-0lax">string</td>
    <td class="tg-0lax">84000</td>
  </tr>
  <tr>
    <td class="tg-0lax">11</td>
    <td class="tg-0lax">checkin</td>
    <td class="tg-0lax">วันเข้าพัก</td>
    <td class="tg-0lax">string</td>
    <td class="tg-0lax">2023-01-05</td>
  </tr>
  <tr>
    <td class="tg-0lax">12</td>
    <td class="tg-0lax">checkout</td>
    <td class="tg-0lax">วันออก</td>
    <td class="tg-0lax">string</td>
    <td class="tg-0lax">2023-01-06</td>
  </tr>
  <tr>
    <td class="tg-0lax">13</td>
    <td class="tg-0lax">payment</td>
    <td class="tg-0lax">หลักฐานการโอนเงิน</td>
    <td class="tg-0lax">string</td>
    <td class="tg-0lax">เป็นข้อมูลแบบ Base64</td>
  </tr>
  <tr>
    <td class="tg-0lax">14</td>
    <td class="tg-0lax">zone</td>
    <td class="tg-0lax">จุดจองเต็นท์</td>
    <td class="tg-0lax">string</td>
    <td class="tg-0lax">zone2</td>
  </tr>
</tbody>
</table><br>

Data Dictionary เก็บข้อมูลของ Equipment หรืออุปกรณ์ที่อำนวยความสะดวกต่างๆ มี Attribute หลายตัว<br>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky">#</th>
    <th class="tg-0pky">Attribute</th>
    <th class="tg-0pky">Description</th>
    <th class="tg-0pky">Data Type</th>
    <th class="tg-0pky">Example</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">1</td>
    <td class="tg-0pky">hanginglamp</td>
    <td class="tg-0pky">โคมไฟห้อย</td>
    <td class="tg-0pky">string</td>
    <td class="tg-0pky">40</td>
  </tr>
  <tr>
    <td class="tg-0pky">2</td>
    <td class="tg-0pky">torch</td>
    <td class="tg-0pky">ไฟฉาย</td>
    <td class="tg-0pky">string</td>
    <td class="tg-0pky">20</td>
  </tr>
  <tr>
    <td class="tg-0pky">3</td>
    <td class="tg-0pky">illumination</td>
    <td class="tg-0pky">ไฟส่องสว่าง</td>
    <td class="tg-0pky">string</td>
    <td class="tg-0pky">80</td>
  </tr>
  <tr>
    <td class="tg-0pky">4</td>
    <td class="tg-0pky">electricity</td>
    <td class="tg-0pky">ไฟฟ้า</td>
    <td class="tg-0pky">string</td>
    <td class="tg-0pky">150</td>
  </tr>
  <tr>
    <td class="tg-0pky">5</td>
    <td class="tg-0pky">privateBathroom</td>
    <td class="tg-0pky">ห้องน้ำส่วนตัว</td>
    <td class="tg-0pky">string</td>
    <td class="tg-0pky">50</td>
  </tr>
  <tr>
    <td class="tg-0pky">6</td>
    <td class="tg-0pky">sharedBathroom</td>
    <td class="tg-0pky">ห้องน้ำรวม</td>
    <td class="tg-0pky">string</td>
    <td class="tg-0pky">20</td>
  </tr>
  <tr>
    <td class="tg-0pky">7</td>
    <td class="tg-0pky">charCoalGrill</td>
    <td class="tg-0pky">เตาปิ้งแบบถ่าน</td>
    <td class="tg-0pky">string</td>
    <td class="tg-0pky">50</td>
  </tr>
  <tr>
    <td class="tg-0pky">8</td>
    <td class="tg-0pky">electricToaster</td>
    <td class="tg-0pky">เตาปิ้งแบบไฟฟ้า</td>
    <td class="tg-0pky">string</td>
    <td class="tg-0pky">60</td>
  </tr>
  <tr>
    <td class="tg-0pky">9</td>
    <td class="tg-0pky">wifi</td>
    <td class="tg-0pky">WIFI</td>
    <td class="tg-0pky">string</td>
    <td class="tg-0pky">50</td>
  </tr>
  <tr>
    <td class="tg-0pky">10</td>
    <td class="tg-0pky">foldingTablehigh</td>
    <td class="tg-0pky">โต๊ะพับสูง</td>
    <td class="tg-0pky">string</td>
    <td class="tg-0pky">30</td>
  </tr>
  <tr>
    <td class="tg-0pky">11</td>
    <td class="tg-0pky">campingSleepingBag</td>
    <td class="tg-0pky">ถุงนอนตั้งแคมป์</td>
    <td class="tg-0pky">string</td>
    <td class="tg-0pky">50</td>
  </tr>
  <tr>
    <td class="tg-0pky">12</td>
    <td class="tg-0pky">foldingChair</td>
    <td class="tg-0pky">เก้าอี้พับ</td>
    <td class="tg-0pky">string</td>
    <td class="tg-0pky">30</td>
  </tr>
</tbody>
</table><br>

ส่วนใหญ่จะเก็บข้อมูลเป็น string ดังนั้นแล้วเมื่อนำข้อมูลไปใช้ในการคำนวณ ในส่วนของ Javascript จึงใช้ Number() ในการแปลงข้อมูลจาก string เป็น int<br><br>

อธิบายเกี่ยวกับ Data Dictionary<br>
id คือ Key ที่เก็บค่า id ของรายการจองเต็นท์<br>
firstname คือ Key ที่เก็บชื่อจริงของผู้จอง<br>
lastname คือ Key ที่เก็บนามสกุลของผู้จอง<br>
phonenumber คือ Key ที่เก็บเบอร์โทรศัพท์ของผู้จอง<br>
idcard คือ Key ที่เก็บหมายเลขบัตรประชาชนของผู้จอง<br>
address คือ Key ที่เก็บที่อยู่ของผู้จอง<br>
subdistrict คือ Key ที่เก็บตำบลของผู้จอง<br>
district คือ Key ที่เก็บอำเภอของผู้จอง<br>
province คือ Key ที่เก็บจังหวัดของผู้จอง<br>
postcode คือ Key ที่เก็บรหัสไปรษณีย์ของผู้จอง<br>
checkin คือ Key ที่เก็บวันเข้าพักของผู้จอง<br>
checkout คือ Key ที่เก็บวันออกของผู้จอง<br>
payment คือ Key ที่เก็บหลักฐานการโอนเงินของผู้จอง<br>
zone คือ Key ที่เก็บจุดที่ผู้จองเต้นท์ได้จองโซนกางเต็นท์<br>
equipment คือ Key ที่เก็บการเช่ายืมอุปกรณ์ที่อำนวยความสะดวกต่างๆ ซึ่งมีให้เลือกหลากหลาย ดังนั้นแล้วจึงต้องจัดเก็บเป็น JSON Object ซึ่งมีข้อมูลดังนี้
- hanginglamp คือ Key ที่เก็บการเช่ายืมโคมไฟห้อยของผู้จอง ซึ่งจะเก็บเป็นราคา โดยเก็บราคาที่ 40 บาท<br>
- torch คือ Key ที่เก็บการเช่ายืมไฟฉายของผู้จอง ซึ่งจะเก็บเป็นราคา โดยเก็บราคาที่ 20 บาท<br>
- illumination คือ Key ที่เก็บการเช่ายืมไฟส่องสว่างของผู้จอง ซึ่งจะเก็บเป็นราคา โดยเก็บราคาที่ 80 บาท<br>
- electricity คือ Key ที่เก็บการเช่ายืมไฟฟ้าของผู้จอง ซึ่งจะเก็บเป็นราคา โดยเก็บราคาที่ 150 บาท<br>
- privateBathroom คือ Key ที่เก็บการเช่ายืมห้องน้ำส่วนตัวของผู้จอง ซึ่งจะเก็บเป็นราคา โดยเก็บราคาที่ 50 บาท<br>
- sharedBathroom คือ Key ที่เก็บการเช่ายืมห้องน้ำรวมของผู้จอง ซึ่งจะเก็บเป็นราคา โดยเก็บราคาที่ 20 บาท<br>
- charCoalGrill คือ Key ที่เก็บการเช่ายืมเตาปิ้งแบบถ่านของผู้จอง ซึ่งจะเก็บเป็นราคา โดยเก็บราคาที่ 50 บาท<br>
- electricToaster คือ Key ที่เก็บการเช่ายืมเตาปิ้งแบบไฟฟ้าของผู้จอง ซึ่งจะเก็บเป็นราคา โดยเก็บราคาที่ 60 บาท<br>
- wifi คือ Key ที่เก็บการเช่ายืม WIFI ของผู้จอง ซึ่งจะเก็บเป็นราคา โดยเก็บราคาที่ 50 บาท<br>
- foldingTablehigh คือ Key ที่เก็บการเช่ายืมโต๊ะพับสูงของผู้จอง ซึ่งจะเก็บเป็นราคา โดยเก็บราคาที่ 30 บาท<br>
- campingSleepingBag คือ Key ที่เก็บการเช่ายืมถุงนอนตั้งแคมป์ของผู้จอง ซึ่งจะเก็บเป็นราคา โดยเก็บราคาที่ 50 บาท<br>
- foldingChair คือ Key ที่เก็บการเช่ายืมเก้าอี้พับของผู้จอง ซึ่งจะเก็บเป็นราคา โดยเก็บราคาที่ 30 บาท<br>
# รายชื่อสมาชิก<br>
1. 64114069 เศรษฐพงษ์ เคียนเขา<br>
2. 64109010 พงษ์นภัส ชูช่วย<br>
3. 64111412 เมธานุสรณ์ สุทธิรัตน์<br>
เทคโนโลยีสารสนเทศและนวัตกรรมดิจิทัล (ITD)
