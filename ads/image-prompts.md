# Prompt สร้างรูปภาพโฆษณา · เก้าอี้โยก

ไฟล์นี้คือ prompt สำหรับสร้างรูป ใช้กับ Nano Banana / Gemini / ChatGPT / Midjourney / Sora
prompt ตัวรูปเขียนเป็นภาษาอังกฤษเพราะโมเดลเข้าใจแม่นกว่า คำอธิบายรอบ ๆ เป็นไทย

> **ข้อสำคัญ ห้ามให้ AI เขียนตัวหนังสือไทยลงบนรูป**
> โมเดลสะกดไทยเพี้ยนเกือบทุกครั้ง สระลอย วรรณยุกต์ผิดที่ ให้สร้างรูปเปล่า ๆ
> แล้วไปพิมพ์ข้อความทับใน Canva หรือ Photoshop เอง จะคุมฟอนต์กับโลโก้ได้ด้วย

---

## 0. บล็อกคุมความสม่ำเสมอ (วางต่อท้ายทุก prompt)

ถ้าไม่ใส่บล็อกนี้ รูปแต่ละใบจะดูเหมือนคนละที่ ทำให้เพจดูไม่น่าเชื่อถือ

```
STYLE LOCK: Documentary-style photograph of a small Thai elderly care home
located in a converted two-story detached house in a Bangkok suburb.
Shot on a 35mm lens, natural daylight from large windows, soft warm light,
gentle shadows, realistic skin texture, candid and unposed.
Color palette: warm wood brown, cream, off-white walls, soft sage green accents,
dusty pink linens. Clean, uncluttered, homey — NOT a hospital, NOT a clinic.
All residents are Thai seniors aged 70-90. All staff are Thai women aged 25-40
wearing light blue or mint polo shirts with navy trousers.
No text, no letters, no logos, no watermarks anywhere in the image.
```

**Negative prompt** (ช่องสำหรับใส่สิ่งที่ไม่เอา ถ้าโมเดลมี)

```
text, letters, thai script, watermark, logo, signage,
hospital ward, IV drips, medical monitors, wheelchairs everywhere,
sad faces, crying, dark gloomy lighting, cold blue tint, clutter,
plastic look, over-smoothed skin, extra fingers, deformed hands,
western faces, young models, cartoon, 3d render, illustration
```

---

## 1. แก้ไขจากรูปเดิม (image-to-image)

ใช้เมื่อมีรูปจริงของศูนย์อยู่แล้ว แต่อยากให้สว่างขึ้น สะอาดขึ้น หรือครอปใหม่
วิธีนี้ปลอดภัยที่สุด เพราะสถานที่ยังเป็นของจริง

```
Using the attached photo as the base, keep the building, room layout,
furniture, and all people's faces exactly as they are — do not replace
or restyle anyone. Only improve the photography:
- lift shadows and brighten the interior with natural window light
- correct white balance to a warm neutral tone
- remove distracting clutter (cables, bins, stray objects) if any
- keep the original composition and framing
Output a clean, realistic photograph. No text, no logo, no watermark.
```

ครอปเป็นสัดส่วนอื่นโดยไม่เสียของ

```
Re-frame the attached photo to a vertical 4:5 crop for a Facebook feed ad.
Extend the scene naturally at the top and bottom (outpaint) to fit the new
ratio, matching the existing lighting, flooring, and wall color exactly.
Do not alter any person, face, or piece of furniture already in the photo.
No text in the image.
```

---

## 2. รูปหน้าบ้าน — จุดขาย "บรรยากาศบ้านเดี่ยว"

ใช้เป็นภาพหลักของแคมเปญ สื่อว่าไม่ใช่ตึก

```
A clean white two-story detached Thai house on a quiet suburban soi in
Bangkok, seen straight-on from the street in the late morning.
Terracotta-tiled carport, white balustrade balcony on the second floor,
grey paving stone driveway, a low white wall with a small flower bed of
green shrubs and soft blue and yellow flowers, a black lantern lamp on
the gatepost, a mature tree on the right, bright cloudy sky.
The house looks freshly painted, quiet, private, well cared for —
a family home, not an institution.
[+ STYLE LOCK]
```

ทางเลือกช่วงเย็น ใช้ทำโพสต์ "เยี่ยมชมได้ถึง 5 โมงเย็น"

```
Same white two-story Thai house, photographed in warm golden late-afternoon
light around 4pm, long soft shadows across the driveway, warm interior
lights just turning on behind the carport, welcoming and calm.
[+ STYLE LOCK]
```

---

## 3. รูปฝึกเดิน — จุดขาย "ดูแลใกล้ชิด 24 ชม." (แนวตั้ง 4:5 / 9:16)

รูปแบบนี้ใช้ทำ Reels และ Story ได้ด้วย

```
Vertical portrait photograph. A Thai grandmother in her early 80s with short
grey hair, wearing a light blue linen button-up shirt and navy trousers,
walking slowly between two stainless-steel parallel handrails in a bright
tiled corridor. She holds the rail with both hands and is smiling slightly,
looking down at her own feet in concentration.
Beside her, a Thai female caregiver in her early 30s in a mint polo shirt
supports her forearm with one hand, the other hand hovering close but not
gripping — attentive, patient, protective. The caregiver is smiling at her,
not at the camera.
In the soft background, an elderly Thai man sits calmly on a wooden chair.
Large windows with dark wooden frames flood the corridor with daylight.
[+ STYLE LOCK]
```

---

## 4. รูปห้องพัก — จุดขาย "เตียงจริงที่ท่านจะได้นอน"

```
A bright, airy shared bedroom in a Thai elderly care home, with three
adjustable hospital-style beds with white frames, made up with clean
dusty-pink and cream bed linen. Polished dark hardwood floor reflecting the
window light, floor-to-ceiling windows with cream curtains and privacy
curtain rails between beds, a small white bedside cabinet per bed,
a view of a green garden outside.
Two Thai grandmothers in their late 70s sit on the edge of their own beds
facing each other, chatting and laughing warmly — relaxed, at home,
not patients. The room is spotless and smells-clean looking, uncrowded,
with plenty of space between beds.
[+ STYLE LOCK]
```

---

## 5. รูปกิจกรรม — จุดขาย "ไม่ได้นอนเฉย ๆ"

```
A warm, lively common room in a Thai elderly care home during a morning
art activity. Eight Thai seniors aged 70-90 sit around two long tables
covered with cream tablecloths, painting watercolor flowers on sketchpads.
Jars of colored water, boxes of pastels, small wooden easels, and a vase of
yellow flowers sit on the tables.
Two Thai female caregivers in light blue polo shirts lean in beside the
seniors, one showing a color box, one gently guiding a brush — both smiling
genuinely. One elderly man sits slightly apart in a wooden rocking chair
by the window, sketching contentedly.
Warm light wood floor, white walls with framed certificates, a large window
with green leaves outside, an orange leather sofa at the back.
The mood is unhurried, social, and cheerful.
[+ STYLE LOCK]
```

---

## 6. รูปเสริม ที่ควรมีไว้เติมแคมเปญ

**อาหาร 3 มื้อ** — ตอบข้อกังวลว่า "ให้กินอะไร"

```
Overhead close-up of a simple, healthy Thai meal for an elderly resident on a
white ceramic plate set on a wooden tray: soft steamed jasmine rice, clear
vegetable soup with tofu, gently steamed fish, finely chopped stir-fried
vegetables, a small dish of sliced ripe papaya, and a glass of water.
Everything looks soft, low-salt, easy to chew, freshly cooked at home —
homestyle cooking, not restaurant plating, not hospital tray food.
Natural daylight on a wooden dining table.
[+ STYLE LOCK]
```

**ห้องน้ำปลอดภัย** — ตอบข้อกังวลเรื่องลื่นล้ม

```
A clean, dry, well-lit bathroom in a Thai elderly care home. Stainless-steel
grab bars mounted beside the toilet and along the shower wall, a sturdy white
shower chair, anti-slip floor matting, a handheld shower head at low height,
a small stool, folded cream towels on a shelf.
Everything spotless and completely dry, no clutter, no mold, bright natural
light from a frosted window. No people in the frame.
[+ STYLE LOCK]
```

**ดูแลกลางคืน** — ย้ำคำว่า 24 ชั่วโมง

```
A quiet night scene inside the care home. A Thai female caregiver in a mint
polo shirt walks softly along a dim corridor holding a small notebook,
checking on residents. Warm low night-lights glow along the skirting boards,
a bedroom door stands slightly ajar with a sleeping resident just visible
in soft shadow. Calm, safe, gentle — reassuring rather than eerie.
Low-light photograph, warm amber tones, no harsh flash.
[+ STYLE LOCK]
```

**คุยกับญาติ** — ใช้กับโพสต์ "เยี่ยมชมฟรี ไม่ต้องนัด"

```
A Thai woman in her late 40s in smart casual office clothes sits at a wooden
table with a Thai female caregiver in a light blue polo shirt, both looking
at a care schedule on a clipboard. The caregiver explains, the daughter
listens and nods, relieved. Two glasses of water on the table, a green plant
behind them, bright natural light from a window.
The mood is honest and reassuring — a real conversation, not a sales pitch.
[+ STYLE LOCK]
```

**สวน / พื้นที่นั่งเล่นนอกบ้าน**

```
A small, tidy garden terrace of a Thai suburban house in the morning.
Two Thai seniors sit on a shaded wooden bench under a frangipani tree,
green artificial lawn and potted plants around them, a caregiver in a mint
polo shirt watering plants nearby. Soft dappled morning sunlight,
white balustrade wall in the background, peaceful and quiet.
[+ STYLE LOCK]
```

---

## 7. รูปสำหรับวางข้อความโฆษณา (มีที่ว่างให้พิมพ์ทับ)

สร้างรูปที่ตั้งใจเว้นพื้นที่ไว้ แล้วค่อยเอาไปใส่ข้อความไทยใน Canva

```
Same scene as [เลือกจากข้อ 2-6], composed as a 1080x1080 square advertisement
background. Place the main subject in the lower two-thirds of the frame and
leave the top third as clean, evenly-lit, low-detail negative space
(plain wall or soft sky) so Thai headline text can be added later.
Also keep the bottom 12% simple for a contact bar.
Absolutely no text or lettering generated in the image.
[+ STYLE LOCK]
```

ข้อความที่จะไปพิมพ์ทับเอง เลือกจากชุดนี้ สั้นและอ่านออกบนมือถือ

- บ้านเดี่ยว รับแค่ 10 เตียง
- เยี่ยมชมฟรี ไม่ต้องนัดล่วงหน้า
- มีทั้งรายวันและรายเดือน
- มีคนดูแล 24 ชั่วโมง
- แถบล่าง: `เยี่ยมชมฟรี 08:00-17:00 · โทร 099-569-1442`

กติกาการวางข้อความ ห้ามใส่ราคาบนรูป และให้พื้นที่ตัวอักษรรวมกันไม่เกิน 20% ของภาพ

---

## 8. ขนาดที่ต้องสั่ง

| ใช้ที่ไหน | สัดส่วน | พิกเซล |
|---|---|---|
| ภาพหลักในฟีด | 4:5 | 1080 x 1350 |
| คารูเซล | 1:1 | 1080 x 1080 |
| Story / Reels | 9:16 | 1080 x 1920 |
| ภาพหน้าปกเพจ | 16:9 | 1920 x 1080 |

---

## 9. เช็กก่อนเอารูปไปใช้

- นับนิ้วมือทุกคนในรูป โมเดลพลาดตรงนี้บ่อยที่สุด
- หน้าคนต้องเป็นคนไทย ไม่ใช่หน้าฝรั่งผิวเข้ม
- ห้ามมีตัวหนังสือมั่ว ๆ โผล่บนผนัง ป้าย หรือเสื้อ
- สภาพห้องในรูปต้องใกล้เคียงของจริง อย่าสร้างห้องหรูกว่าที่มี คนมาดูแล้วผิดหวังเสียลูกค้ายิ่งกว่าเดิม
- ถ้าใช้ภาพ AI แทนภาพถ่ายจริง ควรมีภาพถ่ายจริงของศูนย์อย่างน้อย 1-2 ใบในอัลบั้มเพจเสมอ
