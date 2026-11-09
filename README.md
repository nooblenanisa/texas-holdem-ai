# Texas Hold'em AI Poker — Vercel edition

เล่น Texas Hold'em คนเดียวกับ AI 5 คน รวม 6 ที่นั่ง ใช้ชิปจำลองเท่านั้น

## นำขึ้น Vercel
1. แตกไฟล์ ZIP นี้
2. สร้าง repository ใหม่บน https://github.com
3. อัปโหลดไฟล์และโฟลเดอร์ทั้งหมดจากใน ZIP ไปยัง repository (อย่าอัปโหลด ZIP เป็นไฟล์เดียว)
4. เข้า https://vercel.com แล้วเลือก Add New → Project
5. Import repository ที่สร้างไว้
6. ตั้งค่า Framework Preset เป็น Other และ Output Directory เป็น `public` จากนั้นกด Deploy
7. หากต้องการใช้ ChatGPT API ให้เปิด Project → Settings → Environment Variables แล้วเพิ่ม:
   - `OPENAI_API_KEY` = API key ของคุณ
   - `OPENAI_MODEL` = `gpt-4o-mini` (หรือรุ่นที่บัญชี API รองรับ)
8. เลือก Environment ที่ต้องการ กด Save แล้วไป Deployments → Redeploy
9. เปิดโดเมน `.vercel.app` ที่ Vercel ให้มาเพื่อเล่น

## หมายเหตุ
- ไม่ตั้ง API key ก็เล่นได้ด้วย AI พื้นฐานในเกม
- ห้ามใส่ API key ใน `public/index.html` หรือ commit ลง GitHub
- การเรียก ChatGPT API อาจมีค่าใช้จ่ายตามการใช้งาน
- เกมใช้ชิปจำลอง ไม่มีเงินจริง และเป็นต้นแบบที่ยังไม่รองรับ side pot/all-in หลายระดับอย่างครบถ้วน
