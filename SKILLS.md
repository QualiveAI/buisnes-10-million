# Agent skills для премиальных лендингов

Дата проверки: 21.10.2026. Это shortlist для агента, а не команда «установить всё». Выбираем навыки по назначению и проверяем лицензии/содержимое перед установкой.

## Рекомендуемый стек

### 1. UI UX Pro Max — основной дизайн-интеллект
- Репозиторий: https://github.com/nextlevelbuilder/ui-ux-pro-max-skill
- Зачем: помогает подобрать визуальную систему под нишу, палитру, типографику, компоненты и UX-паттерны.
- Установка:
```bash
npx skills add nextlevelbuilder/ui-ux-pro-max-skill --skill ui-ux-pro-max
```

### 2. Anthropic frontend-design — визуальная оригинальность
- Репозиторий: https://github.com/anthropics/skills
- Зачем: направляет агента к выразительным, production-grade интерфейсам вместо шаблонного «AI-стиля».
- Установка:
```bash
npx skills add anthropics/skills --skill frontend-design
```

### 3. Impeccable — критика и полировка интерфейса
- Репозиторий: https://github.com/pbakaus/impeccable
- Зачем: выявление клише, улучшение иерархии, ритма, типографики, цветов и motion.
- Установка (сначала проверь список skills в репозитории, чтобы избежать конфликта имени frontend-design):
```bash
npx skills add pbakaus/impeccable --list
npx skills add pbakaus/impeccable
```

### 4. Frontend UI Engineering — архитектура и responsive
- Репозиторий: https://github.com/addyosmani/agent-skills
- Зачем: компонентная структура, responsive, доступность, качество реализации.
- Установка:
```bash
npx skills add addyosmani/agent-skills --skill frontend-ui-engineering
```

### 5. Web Design Reviewer — независимый аудит
- Репозиторий: https://github.com/github/awesome-copilot
- Зачем: дополнительный review готового интерфейса и рекомендации по улучшению.
- Установка:
```bash
npx skills add github/awesome-copilot --skill web-design-reviewer
```

## Что ставить первым
Для первого прохода достаточно **UI UX Pro Max + Anthropic frontend-design + frontend-ui-engineering**. Затем используй Impeccable и Web Design Reviewer для критики/QA. Избегай двух skills с одинаковым именем, если агент не умеет изолировать их.

## Общий процесс
1. Исследуй нишу и референсы, но не копируй чужой бренд/макет.
2. Выбери одну визуальную концепцию и опиши дизайн-токены.
3. Сформируй структуру и copy wireframe.
4. Реализуй responsive HTML/CSS.
5. Проведи critique pass отдельным навыком.
6. Проверь доступность, производительность, SEO, мобильные скриншоты и реальные CTA.
7. Отчитайся, что реально проверено.

## Источники
- Каталог frontend skills: https://github.com/finfin/awesome-frontend-skills
- Сводный каталог design agent skills: https://github.com/frankxai/awesome-design-agent-skills
- Frontend agent skills / UX foundations: https://github.com/hueyexe/frontend-agent-skills

Каталоги — источники для дальнейшего поиска, а не знак того, что каждый навык качественный или безопасный. Перед установкой проверь SKILL.md, license, инструкции и требуемые доступы.