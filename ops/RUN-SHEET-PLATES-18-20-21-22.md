# פרומפט Cowork — הרצת לוחות 18, 20, 21, 22 (גרסה עצמאית)

**נכתב ע"י מנהל ה-AI, 21.8.** מיועד לסשן `צוות AI תפעול`
— Claude Desktop על Windows.

## למה גרסה שנייה, ומה היה שגוי בראשונה

הגרסה הראשונה שכתבתי היום שלחה את הסשן לשכפל את הריפו ולקרוא את
`media-review/RUN-SHEET-OPS.md`. **בדקתי את הסשן עצמו, וזה לא היה
עובד.** שתי התיקיות היחידות שהוקצו לו הן:

```
תיקיית הגשר בדרייב (הנתיב אצלך; הריפו הזה ציבורי ולכן אינו נוקב בו)
תיקיית ההורדות שלך
```

אין תיקיית ריפו. הסשן היה מנסה לשכפל, נכשל או נוחת במקום שאינו
מוקצה — ובמקרה הרע היה מאלתר. **התיקייה שאני ויתרתי עליה — הגשר
בדרייב — היא אחת משתי התיקיות שהוא כן רואה.** ההנחה שלי הייתה
שגויה, והפרומפט הזה מתקן אותה.

לכן הבלוק המריץ **מוטמע כאן במלואו**, ולא בהפניה. הוא חולץ מכנית
מ-`media-review/RUN-SHEET-OPS.md` (שורות 120-407) — לא הוקלד מחדש,
ולכן לא יכול היה להשתנות בהעתקה.

---

## הפרומפט — להעתיק מכאן ועד סוף המסמך

```
אתה עובד על "האטלס המקראי" של רותם יעקב, מהמחשב שלו.

המשימה, ורק היא: להריץ ארבעה לוחות מצוירים — 18, 20, 21, 22 —
ולמסור את כל התוצרים. אתה לא מנסח, לא בוחר, לא שופט ולא מתקן.

═══════════════════════════════════════════════════
0 · חמישה כללים שאסור להפר, גם אם נראה לך שכדאי
═══════════════════════════════════════════════════

• **אל תשנה מילה בפרומפט שבסעיף 2.** לא לשפר, לא לקצר, לא "לתקן"
  מה שנראה כשגיאת הקלדה, לא להוסיף ולא להשמיט. הנוסח עבר ביקורת של
  צוות AI מדיה; שינוי שלך מבטל את הביקורת. משהו נראה שגוי — עצור
  ודווח.

• **כל גרסה נמסרת, לא רק ה"טובה".** הופקו ארבע גרסאות ללוח אחד —
  ארבעתן נמסרות, ממוספרות. הבחירה בין גרסאות היא של צוות AI מדיה,
  גם כשההבדל נראה לך ברור. אתה מוסר; הם פוסקים.

• **אל תשכפל את הריפו ואל תיגע בגיט.** אין לך תיקיית ריפו, ואינך
  צריך אחת. כל מה שדרוש נמצא בהודעה הזו.

• **חוק אל-תמציא.** אל תמציא שם של מודל, מספר גרסה, תאריך או מידת
  קובץ. מה שאינך יודע — כתוב שאינך יודע. "אינני בטוח" היא תשובה
  טובה ומועילה.

• **בחשבון של רותם: רק יצירת תמונות.** בלי סיסמאות, בלי יצירת
  חשבונות, בלי שינוי הגדרות, בלי רכישות. משהו חריג — **עצור ודווח,
  אל "תתקן".**

═══════════════════════════════════════════════════
1 · תמונת הייחוס — לפני שמריצים
═══════════════════════════════════════════════════

חפש את הקובץ `ATLAS-16.jpg` בתיקיית הגשר:

    G:\...\אטלס\קלוד DELL\plates\ATLAS-16.jpg

**סימן זיהוי מוחלט: הקובץ הנכון שוקל בדיוק 3,842,241 בתים.**
(2528×1696, 300dpi. זהו לוח מערכת המסתור — חתך אנכי, בית מקורה
מעל, דמות אחת זוחלת על ארבע במחילה.)

לא נמצא בגשר? חפש ב-`תיקיית ההורדות שלך`, לפי הגודל בבתים
ולא לפי שם הקובץ — שמות הורדה חסרי משמעות.

**לא נמצא בשום מקום, או שהגודל אינו תואם — עצור ודווח. אל תריץ
עם תמונת ייחוס אחרת.** הסגנון האחיד של הסדרה תלוי בה.

═══════════════════════════════════════════════════
2 · ההרצה — ארבעה לוחות, הודעה אחת
═══════════════════════════════════════════════════

פתח הודעה חדשה במודל יצירת התמונות. **צרף אליה את ATLAS-16.jpg**,
כתוב את שתי השורות האלה, ומיד אחריהן הדבק את כל הבלוק שמתחת:

Match the style, palette, line weight, grain, paper tone and frame
of the attached reference image exactly. Only the subject changes.

--- תחילת הבלוק, מכאן ועד סוף סעיף 2 ---

ATLAS PLATE — FIXED STYLE. This style block is identical for every
plate and must never vary between plates.

WHAT THIS IS: a restrained documentary reconstruction plate, of the
kind printed in a scholarly historical atlas. It is a drawn plate,
not a photograph and not concept art.

PALETTE: muted earth tones only — parchment cream, deep brown ink,
and ONE desaturated accent. No colour outside that range.

ACCENT DISCIPLINE: the single accent is a muted olive-sage green, used
only for vegetation. Nothing else in the image carries colour. Clothing,
water, roofs and stone stay within the cream-to-brown range. No blue,
no teal, no turquoise anywhere. The figures must never be the most
saturated thing in the frame.

LIGHT: flat, diffuse daylight. No sunset, no sunrise, no golden hour,
no rim light, no dramatic shadow, no visible light source.

CAMERA: eye level, very slightly elevated — the height of a person
standing on the ground. NEVER a bird's-eye view, never looking down into
a building, never an aerial or map-like view. If the whole structure
does not fit at eye level, show only the part that fits.

ROOFS: every building that had a roof is drawn WITH its roof intact.
Do NOT draw a cut-away, a cross-section, or a roofless plan view of any
building, EXCEPT where a plate explicitly asks for one.

SKY: wherever sky is visible it is bare parchment cream, the same tone
as the paper, with no gradient and no cloud. NEVER blue, never tinted,
never atmospheric.

DEPTH BY INTERIOR SHADOW ONLY: the plate is drawn, not pale — but all
of its darkness lives INSIDE forms, never beside them. Go to a deep
near-black brown in these places and these only: the black of an open
doorway or window; the recess under a roof eave or awning; the joints
between stones; the underside of a ledge, step or lintel; the inside of
a niche; the mouth of a jar; the hollow of a rock-cut opening. Model
volume with hatching and cross-hatching, the way an engraved plate
does. Every outward-facing surface is evenly lit across its whole
width.

NOTHING CASTS A SHADOW ONTO ANYTHING ELSE. Specifically, and none of
these may appear: no shadow of an object on the ground or paving beside
it; no shadow of an object on a wall behind it; no diagonal band of
shade across a floor, a wall or a courtyard; no shadow of a roof edge,
awning, fence or parapet; no shadow under or beside a jar, chest,
bench or vessel; no dark side and light side on the same wall. There is
no sun direction anywhere in this image.

FOREGROUND: stage the near edge of the scene deliberately — rocks,
scrub, a broken vessel, the lip of a terrace — drawn with finer detail
and deeper tone than the middle distance, so the eye enters the plate
at the bottom and travels up into it.

FIGURES: only where needed to give scale. Then small, seen from
behind or in profile, never facing the viewer, never a portrait.

SCALE: any human figure stands, kneels or crawls ON THE GROUND at
correct human scale — a head shorter than a doorway, taller than a
storage jar. Never standing on a bench, a wall or furniture. Never
smaller than the vessels beside it.

TEXTURE: fine, even grain across the whole image, like the tooth of
printed paper.

ASPECT: 3:2, horizontal.

NEGATIVE — none of these may appear: photorealism, photograph,
cinematic lighting, golden hour, sunset, sunrise, lens flare, bokeh,
shallow depth of field, wide-angle distortion, dust motes, god rays,
faces toward the viewer, portraits, modern objects, epic scale,
dramatic sky, invented flags, invented emblems, heraldry, epic
atmosphere, saturated colour, HDR, tilt-shift, vignette, aerial view,
bird's-eye view, isometric view, floor plan.

NO WRITING IN ANY IMAGE. The images contain no letters, numbers,
words, labels, captions, titles, plate numbers, signatures,
watermarks, scale bars or compass roses. Do not write "Plate 18",
"Plate 20", "Plate 21", "Plate 22" or any variant in any corner or
along any edge. Where an ancient inscription is part of a depicted object,
render it as illegible incised marks only — never as readable
letters.

OUTPUT — READ THIS CAREFULLY BEFORE GENERATING ANYTHING.

Produce FOUR (4) SEPARATE, INDEPENDENT IMAGES.

This means four distinct image files. It does NOT mean one image
containing four pictures. Do NOT produce a grid, a collage, a contact
sheet, a mood board, a storyboard, a diptych, a triptych, a
side-by-side comparison, a single canvas divided into panels, a sheet
of thumbnails, or any single image containing more than one scene.

Each image contains exactly ONE scene and fills its own complete 3:2
frame, edge to edge.

Generate them ONE AT A TIME, in the order given below. After each
image, state in your written reply which plate it is — in the reply
text only, never inside the image.

Do not write "this concludes", "all images have been generated", "no
plates were skipped", or any similar statement.

End your final reply with two plain lists: the plate numbers you
actually produced as images, and separately, any you did not produce.



PLATE 18.

THIS PLATE'S EXCEPTION: like the hiding-complex plate, this plate is
a cut-away vertical cross-section — here through natural terrain, the
kind of topographic section printed in an expedition report. The cut
is one single straight vertical plane, and sectioned rock carries
dense hatching. Every other rule of the fixed block holds in full.

THE CLAIM OF THIS PLATE: the whole plate exists to show ONE spatial
relationship — the camp sits on the clifftop DIRECTLY ABOVE the cave
mouth, and the cave is unreachable from above and unreachable from
below. Place the rectangular camp outline so that a straight vertical
line dropped from its centre passes through the cave mouth. Between
the camp and the cave there must be nothing but sheer, unbroken
cliff: no path, no ledge system, no stair, no ramp, no rope, no way
down of any kind. Between the cave and the gorge floor, the same —
sheer unbroken rock. This relationship must be unmistakable at a
glance.

SUBJECT: a cross-section of a deep desert canyon. Flat plateau
surfaces run along the top of the frame on both sides, dropping in
sheer high cliff faces to a dry gorge bed at the bottom. High in one
cliff face — well below the plateau rim and far above the gorge floor
— the mouth of a large natural cave opens; its first inner chamber is
shown as a hollow cut by the section plane, its depth sinking to
near-black interior shadow. On the rim directly above the cave, the
small rectangular outline of a military camp enclosure, drawn in pale
elevation. On the opposite rim, a second and smaller camp outline.
The cliff faces carry the fine horizontal bedding lines of desert
rock. The gorge bed is bare and dry, with sparse dry scrub as the
only accent green.

PERIOD MATERIAL: bedded desert limestone, a dry stream bed of pale
boulders, low earthen camp ramparts.

SETTING: desert canyon country; bare parchment sky above the plateau
line.

ADDITIONAL NEGATIVE FOR THIS PLATE: people, soldiers, tents drawn in
detail, ropes, ladders, a path or track of any kind, a dotted route
line, water in the gorge, lush vegetation, palm trees, a sunset,
birds, arrows, leader lines, call-out circles.

DISTINGUISHING FEATURES (all must be present): a sheer-walled canyon
in section dominating the frame vertically; ONE large cave mouth in
the cliff face with its hollow shown in section; a rectangular camp
outline on the rim directly above the cave; a second smaller camp on
the opposite rim; nothing lives and nothing moves in the frame.


ADDITIONAL NEGATIVE FOR THIS PLATE, CONTINUED:
any drawn line, rule, axis, tick or marker added on top of the scene
to indicate a measurement or a relationship; any vertical or
horizontal guide line; any white line anywhere in the image. The
spatial relationship is shown by where things are drawn, never by a
line drawn to point at it.


PLATE 20.

THE CLAIM OF THIS PLATE: what is happening here is a Roman civic
ceremony, not a battle and not a conquest. One man walks behind a
plough drawn by two oxen, cutting a shallow furrow along the ground.
There are no soldiers, no weapons, no armour, no violence, no
prisoners and no fire anywhere in this image. The whole point is that
a city was erased by an administrative act, calmly performed.

SUBJECT: a founding ceremony on cleared, ruined ground. In the middle
distance, seen in profile from the side, a man in a long robe walks
behind a simple wooden plough drawn by a yoked pair of oxen; the fold
of his robe is drawn up over the back of his head. Behind the plough,
a shallow, freshly cut furrow runs across the ground and continues
out of the frame. Two or three other robed figures follow at a
distance, small, seen from behind. Beyond them, the broken walls and
fallen building stone of a destroyed city — low ruined courses, no
standing building, nothing rebuilt.

PERIOD MATERIAL: a plain wooden ard plough, a wooden yoke, undyed
woollen robes, dressed building stone lying fallen and weathered.

SETTING: cleared stony ground on a hilltop, bare parchment sky, low
bare hills beyond the ruins. One or two olive trees at the edge as
the only accent green.

ADDITIONAL NEGATIVE FOR THIS PLATE: soldiers, armour, helmets,
weapons, standards, eagles, a legion, prisoners, chains, violence,
fire, smoke, a temple, a statue of a god, an altar, a crowd, a
throne, a portrait, a face turned toward the viewer, readable letters
of any kind.

DISTINGUISHING FEATURES (all must be present): a wooden plough drawn
by two oxen with a robed man walking behind it; a visible furrow in
the ground behind the plough; low ruined walls of a destroyed city in
the background; not one soldier and not one weapon in the frame.

PLATE 21.

THIS PLATE'S EXCEPTION: this plate is a site plan seen from directly
above — a measured excavation plan of the kind printed in a survey
report. For this plate only, the fixed block's prohibition on an
aerial or map-like view is lifted. The palette, the ink hatching, the
paper grain, the frame and the absolute ban on writing all hold in
full.

THE CLAIM OF THIS PLATE: this is a siege by encirclement, not by
assault. A single continuous siege wall rings the whole spur, closing
it off completely, and the two camps sit outside that ring. There is
NO assault ramp, NO earthen ramp against the defences, NO siege
engine and NO breach anywhere: nothing in this plan may suggest that
the defences were stormed. The plan says: they were shut in and
waited out.

SUBJECT: a plan of a steep triangular rock spur, drawn in fine
hachure relief, isolated between two deep converging valleys and
joined to the hill country behind it by one narrow neck. Along the
spur's edge, a line marking the settlement's own fortification. Set
well back from it, a single continuous thin wall runs right around
the spur, crossing the neck and following the valley slopes, closing
the circuit. On the high ground beyond that wall, to one side, two
plain rectangular camp enclosures, one clearly larger than the other.

PERIOD MATERIAL: dry-stone field walls, low earth and stone ramparts,
rock-cut terrace edges.

SETTING: hill country in plan; the two valleys drawn in hachure
falling away on both sides.

ADDITIONAL NEGATIVE FOR THIS PLATE: an assault ramp, an earthen ramp
against a wall, a siege engine, a battering ram, a catapult, a
breach, a gap in the siege wall, soldiers, tents drawn in detail,
fighting, fire, arrows, leader lines, call-out circles, a north
arrow, a scale bar, any drawn guide line, any white line.

DISTINGUISHING FEATURES (all must be present): a triangular spur
between two valleys with one narrow neck; ONE unbroken siege wall
encircling it completely; TWO rectangular camps outside that wall,
of different sizes; no ramp and no breach anywhere in the plan.

PLATE 22.

THIS PLATE'S EXCEPTION: this plate is a town plan seen from directly
above, like an archaeological phase plan. For this plate only, the
fixed block's prohibition on an aerial or map-like view is lifted.
Everything else in the fixed block holds in full.

THE CLAIM OF THIS PLATE: two cities occupy the same ground and must
read as two clearly different things. The older, destroyed city is
drawn in PALE, BROKEN, DISCONTINUOUS thin lines — fragments of walls
that stop and start, at irregular angles, going nowhere. The new
Roman colony is drawn OVER it in FIRM, DARK, CONTINUOUS lines, ruled
straight, meeting at right angles. A reader must be able to tell at a
glance which lines are the ruin and which are the new grid. If the
two layers read alike, this plate has failed.

SUBJECT: a plan of a walled hilltop town site. Underneath: the pale
broken fragments of the destroyed older city — irregular wall stubs,
scattered, following no single alignment. Over them: a new
rectilinear street grid in firm dark line — one broad main street
running the length of the plan from top to bottom, one broad cross
street meeting it at a right angle, and an open rectangular public
square opening off the main street. Narrower straight lanes divide
the ground between them into regular blocks. The blocks are left
empty — no buildings are drawn inside them.

PERIOD MATERIAL: a plan drawing; the marks are the plate's own ink.

SETTING: the plan fills the frame; bare parchment around it, with
fine hachure indicating the fall of the ground at the edges.

ADDITIONAL NEGATIVE FOR THIS PLATE: drawn buildings, roofs, a temple,
a statue, columns, a city wall drawn as a complete ring, people,
letters or numerals anywhere, a compass rose, a north arrow, a scale
bar, a legend box, arrows, leader lines, colour beyond the fixed
palette.

DISTINGUISHING FEATURES (all must be present): two visually distinct
layers — pale broken fragments beneath, firm dark straight grid over
them; one main street and one cross street meeting at a right angle;
one open rectangular square; empty blocks with no buildings drawn.

--- סוף הבלוק ---

═══════════════════════════════════════════════════
3 · איפה שמים את התוצרים
═══════════════════════════════════════════════════

כל קובץ שהופק — **גם גרסאות שנראות לך פחות טובות** — נשמר אל
תיקיית הגשר, לתת-תיקייה `wip`:

    G:\...\אטלס\קלוד DELL\wip\

(אם `wip` אינה קיימת — צור אותה. זו התיקייה היחידה שמותר לך ליצור.)

בשמות המדויקים האלה:

    ATLAS-18.CANDIDATE-1.jpg
    ATLAS-18.CANDIDATE-2.jpg     (וכן הלאה, לפי מספר הגרסאות)
    ATLAS-20.CANDIDATE-1.jpg
    ATLAS-21.CANDIDATE-1.jpg
    ATLAS-22.CANDIDATE-1.jpg

**אל תיתן לשום קובץ את השם `ATLAS-18.jpg`** (בלי CANDIDATE). השם
הנקי פירושו "עבר ביקורת ומוכן להטמעה", וזו הכרעה של צוות AI מדיה
בלבד. זה הלקח מלוח 16.

**אל תיגע בשום קובץ אחר** בתיקיית הגשר. רק הוספה.

═══════════════════════════════════════════════════
4 · מה לכתוב בדיווח בסוף
═══════════════════════════════════════════════════

בטקסט התשובה (לעולם לא בתוך התמונה), בדיוק את אלה:

  1. רשימת הלוחות שהפקת בפועל כתמונות.
  2. בנפרד — רשימת הלוחות שלא הפקת, ולמה.
  3. כמה גרסאות הופקו לכל לוח, וכמה מהן שמרת. אם המספרים אינם
     שווים — למה.
  4. אם המודל סירב, קטע, או הפיק משהו שאינו ארבע תמונות נפרדות —
     אמור זאת במילים מפורשות. זה מידע שאנחנו צריכים, לא כישלון.
  5. הנתיב המלא שאליו שמרת.

אל תכתוב "כל התמונות הופקו", "לא דולג על אף לוח" או כל משפט סיכום
מרגיע. רשימות בלבד.

**אל תריץ לוח 17 ואל תריץ לוח 19.** 17 ממתין להכרעת הבעלים אחרי
ארבע פסילות על אותו כשל; 19 מיוצר מהנתונים ואינו עובר במודל תמונות
כלל.
```
