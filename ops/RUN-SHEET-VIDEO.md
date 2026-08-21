# דף הרצה — חמישה סרטונים · לצוות AI תפעול

**מנהל ה-AI · 2026-08-20 · לפי הכרעת הבעלים מאותו יום**
**קרא קודם:** `GENERATIVE-VIDEO.md` — במיוחד §1 (הכלל היחיד) ו-§4
(מה אתה מייצר ומה נצרב אחר כך).

> **סטטוס: מאושר להרצה** (צוות AI וידאו, 20.8, הודעה 6 בערוץ) —
> **בכפוף לשלושת התיקונים.** הראשון כבר משוקע בבלוק התנועה שב-§2;
> השניים האחרים ב-**§4ב**, וחובה לקרוא אותם לפני הרצה.
>
> סרטון 1 — מותר להריץ עכשיו: לוח 16 זוהה ואושר. סרטונים 2-5 — עם
> אישור הלוחות שלהם.

---

## 0 · שני דברים לפני הכול

**(א) אתה מוסר פריימים נקיים — בלי אות אחת.** תג המהות, המסגרת
המקווקוות ושורת הגילוי **אינם** נוצרים במודל; הם נצרבים בריפו,
בכלי, מערכים שאפשר לבדוק. אם ראית אות בפריט שחזר — זה פסול, גם אם
היא יפה.

**(ב) שער הקבלה שלך, והוא היחיד:**

> **המצלמה זזה. העולם לא.**
>
> משהו בתוך הפריים זז, נכנס, יוצא, מרצד, מעשן, מתנופף או משנה אור —
> **הקטע נפסל.** לא צריך להיות היסטוריון כדי לשפוט את זה, ולכן זה
> מה שנמסר לידיך. כל השאר — צוות המדיה.

---

## 1 · מה אפשר להריץ מתי — שרשרת התלות

| # | סרטון | לוח הפתיחה | מצב |
|---|---|---|---|
| 1 | מערכת מסתור — הירידה | `ATLAS-16` | **הקובץ קיים.** ממתין לזיהוי צוות המדיה בלבד |
| 2 | מערת האיגרות | `ATLAS-18` | חסום — הלוח טרם הורץ |
| 3 | ביתר | `ATLAS-21` | חסום — הלוח טרם הורץ |
| 4 | המחרשה | `ATLAS-20` | חסום — הלוח טרם הורץ |
| 5 | העיר החדשה | `ATLAS-22` | חסום — הלוח טרם הורץ |

**ארבעת הלוחות החסומים הם בדיוק ארבעת הלוחות שבדף ההרצה של הלוחות**
(`פרומפט-להדבקה-18-20-22.txt` בגשר, ולוח 18 בתוכו). כלומר: **ההרצה
ההיא היא עכשיו גם הנתיב הקריטי של הסרטונים.** קודם הלוחות, אחר כך
הסרטונים מהם.

**סדר עבודה מומלץ:** להריץ את ארבעת הלוחות; למסור ל-`wip/`; ובזמן
שצוות המדיה בודק אותם — להריץ את סרטון 1, שאינו תלוי בהם.

---

## 2 · בלוק התנועה הקבוע — זהה לכל קטע של כל סרטון

הדבק אותו **לפני** שורת הקטע, בכל הרצה, בלי לשנות מילה. **צרף תמיד
תמונת פתיחה** (§3) — סגנון הסדרה נוסע בתמונה, לא בתיאור.

```
MOTION RULES — IDENTICAL FOR EVERY SEGMENT OF EVERY VIDEO.

The attached image is a finished drawn plate from a scholarly historical
atlas. Animate it as a filmed document: THE CAMERA MOVES, THE WORLD DOES
NOT.

Nothing inside the frame changes state. No person enters, leaves, turns,
walks, moves a limb or shifts weight. No animal moves. No object moves,
falls, tips, opens or closes. No wind. No smoke, dust, haze or particles.
No water flows or ripples. No fire, no sparks, no glow. No birds. No
clouds. The light does not change: no shadow moves, no sun direction
appears, no flicker, no lens flare, no vignette pulse.

The drawing itself does not change. Lines are not redrawn, added or
removed. Hatching does not shimmer or crawl. Paper grain is fixed to the
image, not to the screen. Colour and tone stay exactly as in the attached
image throughout.

NO WRITING ANYWHERE. No letters, numbers, words, labels, captions,
titles, plate numbers, signatures, watermarks, scale bars or compass
roses appear at any point, in any frame, in any corner.

CAMERA: one single continuous move, slow and even. No acceleration, no
shake, no handheld float, no snap, no reversal, no rotation. The eight
seconds divide exactly: hold at rest for the FIRST FULL SECOND, move
for the SIX SECONDS between, hold at rest for the LAST FULL SECOND.
The move starts from a dead stop and ends at a dead stop — no drift
into it, no pulse, no bounce, and no jump at either end of the clip.

FRAME: 16:9, 8 seconds. The plate's own drawn frame stays inside the
picture at all times — never crop through it, never lose an edge.

If the move would reveal anything that is not present in the attached
image, stop the move earlier instead of inventing what lies beyond it.
```

---

## 3 · שרשור הקטעים — שני מסלולים

**מסלול א׳ (מועדף):** אם הכלי מקבל תמונת פתיחה — קטע 1 מתחיל מהלוח;
הפריים האחרון של כל קטע הוא תמונת הפתיחה של הבא:

```
ffmpeg -sseof -0.1 -i seg1.mp4 -vframes 1 -q:v 2 seg1-last.jpg
```

**מסלול ב׳ (נסיגה):** אם אינו מקבל — כל קטע מתחיל מהלוח עצמו,
וההרכבה היא חיתוך קשה בין שלושה שוטים. **אל תזייף רציפות בין קטעים
שאינם רציפים.** חיתוך ישר הוא כן; דהייה שמנסה להסתיר קפיצה נתפסת
בעין.

**דווח באיזה מסלול היית.** זה משנה את ההרכבה אצלי.

---

## 4 · חמשת הסרטונים — שורת הקטע

לכל קטע: בלוק התנועה של §2, ואז השורה הזאת בלבד.

### סרטון 1 · מערכת מסתור — הירידה · לוח `ATLAS-16`

```
SEGMENT 1 OF 3. Begin on the whole plate, edge to edge. Push in slowly
and evenly toward the upper third of the image — the village house and
the ground line above the rock. End the move with the house and the
ground line filling the upper half, and hold there at rest.
```
```
SEGMENT 2 OF 3. Begin where the previous clip ended. Move the camera
straight downward, slowly and evenly, following the vertical shaft from
the floor of the house down through the rock. End with the low crawl
tunnel centred in the frame, and hold there at rest.
```
```
SEGMENT 3 OF 3. Begin where the previous clip ended. Pull back slowly
and evenly until the whole plate is visible again, edge to edge, exactly
as in the attached reference. Hold there at rest.
```

**הערה לצוות המדיה, לא לתפעול:** `VIDEO-DESIGN §7` מגדיר לתרשים החתך
תנועה אנכית אחת רציפה **ללא עצירות**, עם הארה נעה על חמשת הרכיבים.
חלוקה לשלושה קטעים מחייבת מנוחה בקצה כל קטע, וההארה היא ממילא שכבת
על שנצרבת אצלי ולא נוצרת במודל. **הסתירה אמיתית ומדווחת** — הכרעה
של צוות AI עיצוב: האם החתך הוא סרטון מנוע לפי §7, סרטון גנרטיבי לפי
כאן, או שניהם לשני שימושים.

### סרטון 2 · מערת האיגרות · לוח `ATLAS-18`

```
SEGMENT 1 OF 3. Begin on the whole plate, edge to edge. Push in slowly
and evenly toward the cliff face on the side where the cave opens. End
with the cliff face filling most of the frame and the cave mouth clearly
inside it, and hold there at rest.
```
```
SEGMENT 2 OF 3. Begin where the previous clip ended. Continue in slowly
and evenly until the cave mouth and its sectioned inner chamber fill the
frame. Hold there at rest.
```
```
SEGMENT 3 OF 3. Begin where the previous clip ended. Pull back slowly
and evenly, straight out, until the whole plate is visible again — the
gorge floor below and the camp outline on the rim above both inside the
frame. Hold there at rest.
```

### סרטון 3 · ביתר — הטבעת שנסגרה · לוח `ATLAS-21`

```
SEGMENT 1 OF 3. Begin on the whole plan, edge to edge. Push in slowly
and evenly toward the centre of the triangular spur, keeping the plan
flat and square to the camera at all times — no tilt, no perspective, no
rotation. Hold at rest at the end.
```
```
SEGMENT 2 OF 3. Begin where the previous clip ended. Drift the camera
slowly and evenly sideways, following the line of the encircling wall,
keeping the plan flat and square to the camera. Hold at rest at the end.
```
```
SEGMENT 3 OF 3. Begin where the previous clip ended. Pull back slowly
and evenly until the whole plan is visible again, edge to edge, flat and
square to the camera. Hold there at rest.
```

### סרטון 4 · המחרשה · לוח `ATLAS-20`

```
SEGMENT 1 OF 3. Begin on the whole plate, edge to edge. Push in slowly
and evenly toward the plough and the pair of oxen in the middle
distance. The man, the oxen and the plough remain completely still — the
camera approaches them, they do not move. Hold at rest at the end.
```
```
SEGMENT 2 OF 3. Begin where the previous clip ended. Drift the camera
slowly and evenly along the cut furrow, away from the plough and toward
the ruined walls beyond. Nothing in the frame moves. Hold at rest at the
end.
```
```
SEGMENT 3 OF 3. Begin where the previous clip ended. Pull back slowly
and evenly until the whole plate is visible again, edge to edge. Hold
there at rest.
```

### סרטון 5 · העיר החדשה על החורבות · לוח `ATLAS-22`

```
SEGMENT 1 OF 3. Begin on the whole plan, edge to edge. Push in slowly
and evenly toward the crossing of the two broad streets, keeping the
plan flat and square to the camera — no tilt, no perspective, no
rotation. Hold at rest at the end.
```
```
SEGMENT 2 OF 3. Begin where the previous clip ended. Drift the camera
slowly and evenly along the main street, from one end of the plan toward
the open rectangular square, keeping the plan flat and square to the
camera. Hold at rest at the end.
```
```
SEGMENT 3 OF 3. Begin where the previous clip ended. Pull back slowly
and evenly until the whole plan is visible again, edge to edge, flat and
square to the camera. Hold there at rest.
```

---

## 4ב · שני תיקוני חובה של צוות AI וידאו — קרא לפני שאתה מריץ

הנוסחים ב-§4 **אושרו** (הודעה 6 בערוץ הווידאו), בשלושה תיקונים.
הראשון כבר בתוך בלוק התנועה שלמעלה. אלה השניים הנותרים.

### תיקון 2 · פתיחות מסלול ב׳

שורות הקטע 2-3 פותחות ב-`Begin where the previous clip ended` — נוסח
שנכון **רק במסלול א׳** (שרשור פריימים). אם אתה במסלול ב׳, החלף את
משפט הפתיחה בלבד; כל שאר השורה נשארת כלשונה.

| קטע | פתיחת מסלול ב׳ |
|---|---|
| סרטון 1 · קטע 2 | `Begin framed on the vertical shaft below the house floor, the shaft centred.` |
| סרטון 1 · קטע 3 | `Begin framed on the low crawl tunnel, centred.` |
| סרטון 2 · קטע 2 | `Begin with the cliff face filling most of the frame and the cave mouth inside it.` |
| סרטון 2 · קטע 3 | `Begin with the cave mouth and its sectioned inner chamber filling the frame.` |
| סרטון 3 · קטע 2 | `Begin framed on the centre of the triangular spur.` |
| סרטון 3 · קטע 3 | `Begin framed on a stretch of the encircling wall.` |
| סרטון 4 · קטע 2 | `Begin framed on the plough and the pair of oxen in the middle distance.` |
| סרטון 4 · קטע 3 | `Begin framed on the ruined walls at the far end of the furrow.` |
| סרטון 5 · קטע 2 | `Begin framed on the crossing of the two broad streets.` |
| סרטון 5 · קטע 3 | `Begin framed on the open rectangular square.` |

### תיקון 3 · שער תוכן-הלוח — **שער שני שנמסר לשיפוטך**

שורות הקטע נוקבות פרטים בתוך הלוחות: צד המערה במצוק, שלוחה משולשת,
חומת הכיתור, המחרשה, שני הרחובות, הכיכר. **לוחות 18 ו-20-22 טרם
הורצו** — הפרטים האלה הם כוונת ההזמנה, לא עובדה על קובץ.

לכן, לפני הרצת כל סרטון: **ודא שהפרט שהשורה נוקבת בו קיים בלוח
המאושר שקיבלת.** אין התאמה — **עצור והחזר לצוות AI וידאו. אל תאלתר
תנועה אחרת.**

זה השער השני שלך, לצד "המצלמה זזה, העולם לא". שניהם נבדקים בעין ובלי
ידע היסטורי, ובדיוק לכן הם שלך.

---

## 5 · מסירה

לתיקיית `wip/` בגשר, בשמות מדויקים:

```
VIDEO-01-seg1.mp4   VIDEO-01-seg2.mp4   VIDEO-01-seg3.mp4
VIDEO-02-seg1.mp4   …
```

**וכמו בלוחות: כל גרסה נמסרת, לא רק ה"טובה".** יצאו שלוש גרסאות
לקטע — `VIDEO-01-seg1-v1.mp4`, `-v2`, `-v3`. הבחירה היא של צוות
המדיה. לוח 16 תקוע היום בדיוק בגלל שנמסרה אחת מתוך ארבע.

**בדוח שלך, לכל קטע:** האם המסלול היה א׳ או ב׳; האורך בפועל בשניות;
וכל דבר שראית זז בפריים — גם אם פסלת אותו והרצת שוב. **התקלות שנפסלו
הן מידע, לא בושה** — הן מה שילמד אותנו אם הכלל בכלל מחזיק.

## 6 · ההרכבה — אצלי, לא אצלך

לידיעתך בלבד, כדי שתדע למה השמות חשובים:

```
ffmpeg -f concat -safe 0 -i segments.txt -c copy VIDEO-01-raw.mp4
```

ואז צריבת המסגרת, תג המהות ושורת הגילוי לפי `VIDEO-DESIGN §9`,
הכתוביות לפי §5, והקריינות לפי §12. **אל תרכיב, אל תצרוב ואל תוסיף
שמע.** תמסור קטעים.

---

**ובחשבון של רותם: רק יצירת תמונות ווידאו.** בלי סיסמאות, בלי יצירת
חשבונות, בלי שינוי הגדרות. משהו חריג — עצור ודווח, אל "תתקן".
