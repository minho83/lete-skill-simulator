# 🎮 뉴 레테 스킬 시뮬레이터 (New Lete Skill Simulator)

A comprehensive skill simulation tool for the New Lete game, featuring 305 unique skills across 14 different categories.

## ✨ Features

- **305 Total Skills**: Complete skill database with detailed information
- **14 Skill Categories**: Organized into Magic, Abilities, and Traits
  - 🔥 화염 마법 (Fire Magic): 11 skills
  - ❄️ 얼음 마법 (Ice Magic): 21 skills
  - ⚡ 번개 마법 (Lightning Magic): 20 skills
  - 🧠 초능력 마법 (Psychic Magic): 13 skills
  - 🌀 융합 마법 (Fusion Magic): 14 skills
  - 💪 힘 능력 (Strength Ability): 21 skills
  - 🏃 민첩 능력 (Agility Ability): 21 skills
  - 🛡️ 보조 능력 (Support Ability): 26 skills
  - ⚖️ 조화 능력 (Harmony Ability): 29 skills
  - ⚔️ 용맹 특성 (Courage Trait): 29 skills
  - 🛡️ 강인 특성 (Fortitude Trait): 28 skills
  - 🏔️ 고독 특성 (Solitude Trait): 28 skills
  - 🎭 교활 특성 (Cunning Trait): 24 skills
  - 🔧 유용 특성 (Utility Trait): 20 skills
- **Interactive Web Interface**: User-friendly skill browser and simulator
- **Detailed Skill Information**: Including names, categories, levels, and descriptions
- **Excel-based Data Management**: Easy to update and maintain

## 🚀 GitHub Pages 배포 가이드

### 1단계: GitHub 저장소 생성
1. [GitHub](https://github.com)에 로그인
2. 우측 상단의 **+** 버튼 클릭 → **New repository** 선택
3. 저장소 이름 입력 (예: `lete-skill-simulator`)
4. **Public** 선택 (GitHub Pages 무료 사용을 위해)
5. **Create repository** 클릭

### 2단계: 로컬 저장소를 GitHub에 연결
```bash
# 원격 저장소 추가 (your-username을 본인의 GitHub 사용자명으로 변경)
git remote add origin https://github.com/your-username/lete-skill-simulator.git

# 기본 브랜치를 main으로 설정
git branch -M main

# GitHub에 푸시
git push -u origin main
```

### 3단계: GitHub Pages 활성화
1. GitHub 저장소 페이지로 이동
2. **Settings** 탭 클릭
3. 왼쪽 메뉴에서 **Pages** 클릭
4. **Source** 섹션에서:
   - **Branch** 선택: `main`
   - **Folder** 선택: `/ (root)`
5. **Save** 버튼 클릭

### 4단계: 웹사이트 접속
- 몇 분 후 다음 주소로 접속 가능:
  - `https://your-username.github.io/lete-skill-simulator/`
- 배포 상태는 저장소의 **Settings → Pages**에서 확인 가능

### 📝 참고사항
- `index.html` 파일이 루트 디렉토리에 있어야 자동으로 인식됩니다
- 변경사항을 푸시하면 자동으로 웹사이트가 업데이트됩니다 (몇 분 소요)
- 커스텀 도메인도 설정할 수 있습니다


## 🌐 Live Demo

Access the web demo: [https://www.genspark.ai/api/files/s/EMtILTu8](https://www.genspark.ai/api/files/s/EMtILTu8)

## 🛠️ Technology Stack

- **Data Management**: Microsoft Excel / Google Sheets
- **Web Interface**: HTML, CSS, JavaScript
- **Data Format**: JSON (exported from Excel)

## 📊 Data Structure

The skill database is organized in the following structure:


Clean Skill Data:
  Column A: Image# (Image identifier)
  Column B: Skill Name (Korean skill name)
  Column C: Category (Skill category)
  Column D: Max Level (Maximum skill level)
  Column E-H: Additional skill properties
  Total Rows: 324 (including headers)


### Skill Categories Breakdown

| Category Type | Category Name | Skill Count |
|--------------|---------------|-------------|
| Magic | 화염 마법 (Fire Magic) | 11 |
| Magic | 얼음 마법 (Ice Magic) | 21 |
| Magic | 번개 마법 (Lightning Magic) | 20 |
| Magic | 초능력 마법 (Psychic Magic) | 13 |
| Magic | 융합 마법 (Fusion Magic) | 14 |
| Ability | 힘 능력 (Strength) | 21 |
| Ability | 민첩 능력 (Agility) | 21 |
| Ability | 보조 능력 (Support) | 26 |
| Ability | 조화 능력 (Harmony) | 29 |
| Trait | 용맹 특성 (Courage) | 29 |
| Trait | 강인 특성 (Fortitude) | 28 |
| Trait | 고독 특성 (Solitude) | 28 |
| Trait | 교활 특성 (Cunning) | 24 |
| Trait | 유용 특성 (Utility) | 20 |
| **Total** | | **305** |

## 📁 File Structure


뉴 레테 스킬 시뮬레이터 - 24.03.27.xlsx
├── 스킬 시뮬레이터 (Skill Simulator Sheet)
├── Web Data Structure (Web export format)
├── Clean Skill Data (Clean organized data)
└── GitHub README (This documentation)


## 🚀 Setup Instructions

### For Excel/Sheets Users

1. Download the file: `뉴 레테 스킬 시뮬레이터 - 24.03.27.xlsx`
2. Open with Microsoft Excel or Google Sheets
"3. Navigate to the ""스킬 시뮬레이터"" sheet to view the main simulator"
"4. Use ""Clean Skill Data"" sheet for raw data access"

### For Web Developers

"1. Export ""Web Data Structure"" sheet to JSON format"
2. Integrate the JSON data with your web application
3. Reference the live demo for UI/UX implementation ideas


// Example: Loading skill data from exported JSON
const skillsData = await loadSkillsFromExport();
// Process 305 skills across 14 categories
console.log(`Loaded ${skillsData.length} skills`);


## 📖 Usage Guide

### Viewing Skills

"1. Open the ""스킬 시뮬레이터"" sheet"
2. Browse skills by category
3. View detailed information including max levels and descriptions

### Adding New Skills

"1. Navigate to ""Clean Skill Data"" sheet"
2. Add a new row with the following information:
   - Image# (unique identifier)
   - Skill Name (Korean)
   - Category (one of the 14 categories)
   - Max Level (maximum achievable level)
   - Additional properties
3. Update category count statistics if adding to a new category

### Exporting Data

"1. Use ""Web Data Structure"" sheet for web-ready format"
2. Export as CSV or JSON for external applications
3. Maintain data integrity by preserving column structure

## 🎯 Key Statistics

- **Total Skills**: 305
- **Categories**: 14
- **Skill Types**: Magic (5 categories), Abilities (4 categories), Traits (5 categories)
- **Data Version**: 24.03.27
- **Language**: Korean with English translations

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Report Issues**: Found incorrect skill data? Open an issue
2. **Suggest Features**: Have ideas for new features? Share them
3. **Update Skills**: New game version? Submit updated skill information
4. **Improve Documentation**: Help make this README better

### Guidelines

- Maintain Korean skill names as primary with English translations
"- Follow the existing data structure in ""Clean Skill Data"""
- Test changes thoroughly before submitting
- Update category counts when adding/removing skills

## 📝 License

This project is created for the New Lete gaming community. Please respect the intellectual property of the original game content.

## 📞 Contact & Support

For questions, suggestions, or support:
- Check the live demo: [https://www.genspark.ai/api/files/s/EMtILTu8](https://www.genspark.ai/api/files/s/EMtILTu8)
- Review the Excel file for detailed data

---

**Last Updated**: March 27, 2024
**Total Skills**: 305 across 14 categories
**Version**: 24.03.27

Made with ❤️ for the New Lete community
