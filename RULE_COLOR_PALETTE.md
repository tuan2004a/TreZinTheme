# Rule: Color Palette
> **Quy tắc tối ưu cho việc thiết theme vscode**

---
## 1. Triết Lý Thiết Kế

### Nguyên Tắc Cốt Lõi
1. **Dark-First**: Giảm độ chói tổng thể, dễ chịu khi nhìn 2-4 giờ liên tục
2. **Code-Focused**: Syntax highlighting rõ ràng, dễ đọc
3. **Minimal Distraction**: UI tối giản, tập trung vào nội dung
4. **Calm Palette**: Màu bão hòa thấp-medium

### Tại Sao Dark Theme?

- Giảm độ chói tổng thể, dễ chịu hơn khi nhìn lâu (đặc biệt ban đêm)
- Tiết kiệm pin trên OLED/AMOLED displays
- Tăng focus khi code/học ban đêm
- Nền tối + accent dịu, highlight có kiểm soát

### Tiêu chuẩn đọc lâu

- Foreground vs Background đủ tương phản (ít nhất mức “dễ đọc”, tránh xám quá nhạt trên nền tối).
- Comment không quá chìm: comment là “thông tin”, không phải “rác thị giác”.
- Tránh dùng quá nhiều màu bão hòa cho text thường; chỉ “bão hòa” khi là trạng thái (error/warn) hoặc điểm nhấn.

---
## 2. Bảng màu(Color Palette Mapping)

### Syntax Role Mapping

- **This keyword, HTML elements, Regex group symbol, CSS units**
- **Number and Boolean constants, Language support constants**
- **Function parameters, Regex character sets**
- **Parameters inside functions**
- **Strings, CSS class names**
- **Object literal keys, Markdown links**
- **Regex literal strings**
- **Language support functions, CSS HTML elements**
- **Object properties, Regex quantifiers and flags, Markdown headings, Markdown code, Import/Export keywords**
- **Function names, CSS property names** 
- **Control Keywords, Storage Types, Regex symbols and operators, HTML Attributes**
- **Variables, Class names**
- **Editor Foreground**
- **Markdown Text, HTML Text** 
- **Comments**
- **Terminal Black**

### Mapping chi tiết

- this keyword → Special keyword / Self reference
- HTML elements / CSS HTML elements (tag name) → Tag name
- HTML attributes → Attribute name
- CSS property names → Property name
- CSS class names (selector .class) → Class selector
- CSS units (px, rem, %, …) → Unit / Literal suffix
- Function names → Function / Method name
- Function parameters (mọi trường hợp) → Parameter
- Variables / identifiers → Variable / Identifier
- Class names / type names → Type / Class / Interface name
- Object properties (obj.prop, field access) → Property / Member
- Object literal keys ({ key: value }, JSON/YAML keys) → Key (Object key)
- Strings → String literal
- Number & Boolean constants + language constants (null/undefined/true/false, …) → Literal / Built-in constant
- Control keywords (if/else/for/return/import/export/async/await, …) → Keyword / Control flow
- Storage types / declarations (class/interface/enum/type/let/const/var, tùy ngôn ngữ) → Storage / Declaration / Type keyword

Regex

- Regex literal/pattern content → Regex pattern
- Regex group symbols ( ) + punctuation → Regex punctuation
- Regex character sets [ ... ] → Regex character set
- Regex quantifiers + flags (* + ? {n} gim…) → Regex quantifier / Flag

Markdown

- Headings → Heading
- Links → Link
- Inline code / code block → Code span / Code block
- Markdown text → Text

General

- Editor foreground → Default text
- HTML text → Text
- Comments → Comment
- Terminal Black → Terminal ANSI base (black)

---
## 3. Quy tắc

- Regex/Warnings nên nổi vừa phải: nổi quá sẽ làm code “nhấp nháy”.
- UI luôn trầm hơn code: để mắt bạn “đi vào code” trước.