# pamusan-blog-writer

Claude skill — Ahrefs entegreli, 800-900 kelimelik SEO blog yazarı.

## Ne Yapar?

- 🔍 Ahrefs MCP ile gerçek zamanlı keyword + rakip analizi
- ✍️ 800-900 kelime, insan gibi yazılmış blog üretir
- 🔗 Ürün ve kategori linklerini doğal anchor'larla yerleştirir
- 🔄 Her blogda farklı anchor metni kullanır, tekrar etmez
- 📊 Her blog sonunda SEO raporu + anchor raporu çıkarır

## Kurulum

Bu klasörü Claude skills dizinine koy:

```
skills/
└── pamusan-blog-writer/
    ├── SKILL.md              ← Ana skill dosyası
    └── references/
        ├── anchor-arsivi.md  ← Kullanılmış anchor'lar (manuel güncelle)
        ├── yasakli-ifadeler.md
        └── blog-ornekleri.md
```

## Kullanım

Claude'a şunları söyle:

```
"[Konu] hakkında blog yaz"
"Kategori: [URL]"
"Ürünler: [URL1], [URL2]"
"Daha önce kullandığım anchor'lar: [liste]"
```

## Gereksinimler

- Claude.ai'da **Ahrefs MCP** bağlı olmalı
- `https://api.ahrefs.com/mcp/mcp` connector aktif

## Anchor Takibi

Her blog yazıldıktan sonra `references/anchor-arsivi.md` dosyasını güncelle.
Bir sonraki blogda o anchor'lar kullanılmaz.

## Klasör Yapısı

```
pamusan-blog-writer/
├── SKILL.md
└── references/
    ├── anchor-arsivi.md
    ├── blog-ornekleri.md
    └── yasakli-ifadeler.md
```
