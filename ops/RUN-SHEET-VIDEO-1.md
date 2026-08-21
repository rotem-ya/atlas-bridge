# דף הרצה — סרטון 1 · מערכת מסתור, הירידה · לצוות AI תפעול

**מנהל ה-AI · 2026-08-21.** דף עצמאי: כל מה שדרוש נמצא כאן, ואין בו
הפניה לקובץ שאין לך. נבנה מכנית ממקור שעבר ביקורת — **אל תשנה מילה.**

> **הסרטון הזה פתוח להרצה עכשיו.** לוח 16 קיים, זוהה ואושר; פסקת
> תנועת המצלמה נסגרה בהכרעת הבעלים ב-21.8 והיא בתוך הבלוק שלמטה
> (מנוחה שנייה אחת · תנועה שש שניות · מנוחה שנייה אחת). ארבעת
> הסרטונים האחרים ממתינים ללוחות שלהם ואינם כאן.

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

## 1 · תמונת הפתיחה — לפני שמריצים

הסרטון נפתח מלוח `ATLAS-16` עצמו. חפש אותו בתיקיית הגשר:

    G:\...\אטלס\קלוד DELL\plates\ATLAS-16.jpg

**סימן זיהוי מוחלט: הקובץ הנכון שוקל בדיוק 3,842,241 בתים.**
(2528×1696. זהו לוח מערכת המסתור — חתך אנכי, בית מקורה מעל, דמות
אחת זוחלת על ארבע במחילה.)

לא נמצא בגשר? חפש בתיקיית ההורדות שלך **לפי הגודל בבתים ולא לפי
השם** — שמות הורדה חסרי משמעות. לא נמצא בשום מקום, או שהגודל אינו
תואם — **עצור ודווח. אל תריץ עם תמונה אחרת.**

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

## 4 · שלושת הקטעים

לכל קטע: בלוק התנועה של סעיף 2 **כלשונו**, ואז שורת הקטע בלבד.

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

---

## 4ב · תיקון חובה של צוות AI וידאו — מסלול ב׳

שורות הקטע 2-3 פותחות ב-`Begin where the previous clip ended` — נוסח
שנכון **רק במסלול א׳** (שרשור פריימים). אם אתה במסלול ב׳, החלף את
משפט הפתיחה בלבד; כל שאר השורה נשארת כלשונה.

| קטע | פתיחת מסלול ב׳ |
|---|---|
| סרטון 1 · קטע 2 | `Begin framed on the vertical shaft below the house floor, the shaft centred.` |
| סרטון 1 · קטע 3 | `Begin framed on the low crawl tunnel, centred.` |

**והשער השני שנמסר לשיפוטך:** שורות הקטע נוקבות פרטים בתוך הלוח —
הבית וקו הקרקע, הפיר האנכי, מחילת הזחילה. ודא שכל פרט קיים בלוח
שקיבלת. אין התאמה — **עצור והחזר. אל תאלתר תנועה אחרת.**

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

---

**ובחשבון של רותם: רק יצירת תמונות ווידאו.** בלי סיסמאות, בלי יצירת
חשבונות, בלי שינוי הגדרות, בלי רכישות. משהו חריג — עצור ודווח,
אל "תתקן".
