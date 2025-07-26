# 🍱 Sushiman - Modern Japanese Restaurant Landing Page

## 📌 프로젝트 개요
**Sushiman**은 일본 음식 문화의 정수를 담은 모던한 랜딩 페이지입니다. 미니멀한 디자인과 부드러운 인터랙션으로 사용자에게 프리미엄 일식 레스토랑의 경험을 전달합니다.

### 🎯 핵심 가치
- **Omotenashi (おもてなし)**: 일본의 환대 정신을 디지털 경험으로 구현
- **Visual Storytelling**: 시각적 요소로 브랜드 스토리 전달
- **Performance First**: 빠른 로딩과 부드러운 애니메이션

## 🛠 기술 스택

### Frontend
- **Pure HTML5 & CSS3**: 프레임워크 없이 순수 웹 표준 기술로 구현
- **Vanilla JavaScript (ES6+)**: 모듈 시스템을 활용한 클린 코드
- **AOS (Animate On Scroll)**: 스크롤 기반 애니메이션으로 몰입감 있는 UX

### Build & Development
- **Vite**: 빠른 HMR과 최적화된 빌드 시스템
- **NPM Scripts**: 간결한 개발 워크플로우

### Design System
- **CSS Custom Properties**: 일관된 디자인 토큰 관리
- **BEM Methodology**: 확장 가능하고 유지보수가 용이한 CSS 아키텍처
- **Modular CSS Architecture**: 섹션별 분리된 스타일시트
- **Responsive Design**: 모바일 퍼스트 접근

## 🏗 프로젝트 구조

```
st-sushi-landing/
├── assets/              # 이미지 및 아이콘 리소스
├── css/
│   ├── style.css       # 글로벌 스타일 및 변수
│   └── sections/       # 컴포넌트별 스타일 모듈
│       ├── header.css
│       ├── hero.css
│       ├── about.css
│       ├── popular.css
│       ├── trending.css
│       ├── subscribe.css
│       └── footer.css
├── js/
│   └── script.js       # 메인 JavaScript 파일
└── index.html          # 메인 HTML
```

## 💡 설계 철학

### 1. **BEM (Block Element Modifier) 방법론**
체계적이고 확장 가능한 CSS 클래스 명명 규칙을 적용하여 컴포넌트 기반 스타일링을 구현했습니다.

```css
/* Block: 독립적인 컴포넌트 */
.hero {}
.popular-foods {}

/* Element: Block의 구성 요소 */
.hero__content {}
.hero__image {}
.popular-foods__card {}
.popular-foods__card-title {}

/* Modifier: Block/Element의 변형 */
.popular-foods__card--active {}
.hero__button--primary {}

/* 실제 적용 예시 */
.header__menu {}
.header__menu-mobile {}
.hero-content__testimonial {}
.popular-foods__filter-btn {}
.trending__arrow--left {}
```

### BEM의 장점
- **명확한 계층 구조**: 클래스명만으로 HTML 구조 파악 가능
- **스타일 충돌 방지**: 네임스페이스로 작동하여 CSS 특정성 문제 해결
- **재사용성**: 독립적인 블록 단위로 컴포넌트 재사용
- **유지보수성**: 일관된 명명 규칙으로 팀 협업 용이

### 2. **Component-Based CSS Architecture**
각 섹션을 독립적인 컴포넌트로 분리하여 유지보수성과 재사용성을 극대화했습니다.

```css
/* 컴포넌트별 독립적인 스타일 관리 */
@import url("sections/header.css");
@import url("sections/hero.css");
@import url("sections/about.css");
```

### 3. **Performance Optimization**
- Vite의 번들 최적화로 빠른 로딩 속도
- 이미지 lazy loading 고려
- CSS 모듈화로 필요한 스타일만 로드

### 4. **Semantic HTML & Accessibility**
- 시맨틱 태그 사용 (header, nav, section, article, footer)
- 적절한 alt 텍스트와 ARIA 레이블
- 키보드 네비게이션 지원

### 5. **Design Tokens System**
```css
:root {
  --primary-color: #b1454a;
  --playfair-display: "Playfair Display", serif;
  --plus-jakarta-sans: "Plus Jakarta Sans", sans-serif;
}
```

## 🎨 주요 기능

### 📱 반응형 디자인
- 모바일, 태블릿, 데스크톱 완벽 대응
- 햄버거 메뉴로 모바일 UX 최적화

### 🎭 인터랙티브 애니메이션
- AOS 라이브러리를 활용한 스크롤 애니메이션
- fade, flip, zoom 효과로 동적인 사용자 경험

### 🔍 SEO 최적화
- Open Graph 메타 태그 구현
- Twitter Card 지원
- 시맨틱 마크업으로 검색엔진 최적화

## 🚀 실행 방법

```bash
# 의존성 설치
npm install

# 개발 서버 실행
npm run dev

# 프로덕션 빌드
npm run build

# 빌드 미리보기
npm run preview
```

## 🌐 배포
- **Production URL**: https://st-sushi-landing.vercel.app
- Vercel을 통한 자동 배포 및 최적화

## 📈 성과 및 학습 포인트

### 기술적 성과
- **순수 웹 기술 마스터**: 프레임워크 없이 모던한 웹사이트 구현
- **BEM 방법론 적용**: 확장 가능하고 유지보수가 용이한 CSS 구조
- **모듈화 설계**: 컴포넌트 기반 아키텍처 구축
- **성능 최적화**: Lighthouse 점수 90+ 달성

### 비즈니스 가치
- **브랜드 아이덴티티**: 일본 문화를 현대적으로 재해석
- **사용자 경험**: 직관적인 네비게이션과 매력적인 비주얼
- **전환율 최적화**: CTA 버튼과 구독 폼으로 리드 생성

## 🔮 향후 개선 계획
- [ ] 다국어 지원 (일본어, 영어)
- [ ] 다크 모드 구현
- [ ] 웹 접근성 강화 (WCAG 2.1 준수)
- [ ] PWA 전환
- [ ] 애니메이션 성능 최적화

---

### 🤝 Contact
이 프로젝트는 모던 웹 개발의 베스트 프랙티스를 따르며, 클린 코드와 확장 가능한 아키텍처를 추구합니다.

---

# 🍱 Sushiman - Modern Japanese Restaurant Landing Page (English Version)

## 📌 Project Overview

**Sushiman** is a modern landing page that captures the essence of Japanese food culture. It delivers a premium Japanese restaurant experience through minimal design and smooth interactions.

### 🎯 Core Values

- **Omotenashi (おもてなし)**: Implementing Japanese hospitality spirit in digital experience
- **Visual Storytelling**: Delivering brand story through visual elements
- **Performance First**: Fast loading and smooth animations

## 🛠 Tech Stack

### Frontend

- **Pure HTML5 & CSS3**: Implementation with pure web standards without frameworks
- **Vanilla JavaScript (ES6+)**: Clean code utilizing module system
- **AOS (Animate On Scroll)**: Immersive UX with scroll-based animations

### Build & Development

- **Vite**: Fast HMR and optimized build system
- **NPM Scripts**: Simple development workflow

### Design System

- **CSS Custom Properties**: Consistent design token management
- **BEM Methodology**: Scalable and maintainable CSS architecture
- **Modular CSS Architecture**: Section-separated stylesheets
- **Responsive Design**: Mobile-first approach

## 🏗 Project Structure

```
st-sushi-landing/
├── assets/              # Image and icon resources
├── css/
│   ├── style.css       # Global styles and variables
│   └── sections/       # Component-specific style modules
│       ├── header.css
│       ├── hero.css
│       ├── about.css
│       ├── popular.css
│       ├── trending.css
│       ├── subscribe.css
│       └── footer.css
├── js/
│   └── script.js       # Main JavaScript file
└── index.html          # Main HTML
```

## 💡 Design Philosophy

### 1. **BEM (Block Element Modifier) Methodology**

Implemented component-based styling by applying systematic and scalable CSS class naming conventions.

```css
/* Block: Independent components */
.hero {}
.popular-foods {}

/* Element: Components of a Block */
.hero__content {}
.hero__image {}
.popular-foods__card {}
.popular-foods__card-title {}

/* Modifier: Variations of Block/Element */
.popular-foods__card--active {}
.hero__button--primary {}

/* Real-world examples */
.header__menu {}
.header__menu-mobile {}
.hero-content__testimonial {}
.popular-foods__filter-btn {}
.trending__arrow--left {}
```

### Benefits of BEM

- **Clear Hierarchy**: Understanding HTML structure through class names alone
- **Prevents Style Conflicts**: Works as namespace to solve CSS specificity issues
- **Reusability**: Component reuse through independent block units
- **Maintainability**: Easy team collaboration with consistent naming conventions

### 2. **Component-Based CSS Architecture**

Maximized maintainability and reusability by separating each section as independent components.

```css
/* Independent style management per component */
@import url("sections/header.css");
@import url("sections/hero.css");
@import url("sections/about.css");
```

### 3. **Performance Optimization**

- Fast loading speed with Vite's bundle optimization
- Considering image lazy loading
- Loading only necessary styles through CSS modularization

### 4. **Semantic HTML & Accessibility**

- Using semantic tags (header, nav, section, article, footer)
- Proper alt text and ARIA labels
- Keyboard navigation support

### 5. **Design Tokens System**

```css
:root {
  --primary-color: #b1454a;
  --playfair-display: "Playfair Display", serif;
  --plus-jakarta-sans: "Plus Jakarta Sans", sans-serif;
}
```

## 🎨 Key Features

### 📱 Responsive Design

- Perfect adaptation for mobile, tablet, and desktop
- Mobile UX optimization with hamburger menu

### 🎭 Interactive Animations

- Scroll animations using AOS library
- Dynamic user experience with fade, flip, zoom effects

### 🔍 SEO Optimization

- Open Graph meta tags implementation
- Twitter Card support
- Search engine optimization with semantic markup

## 🚀 Getting Started

```bash
# Install dependencies
npm install

# Run development server
npm run dev

# Production build
npm run build

# Preview build
npm run preview
```

## 🌐 Deployment

- **Production URL**: <https://st-sushi-landing.vercel.app>
- Automatic deployment and optimization through Vercel

## 📈 Achievements & Learning Points

### Technical Achievements

- **Mastering Pure Web Technologies**: Implementing modern website without frameworks
- **BEM Methodology Application**: Scalable and maintainable CSS structure
- **Modular Design**: Building component-based architecture
- **Performance Optimization**: Achieving Lighthouse score 90+

### Business Value

- **Brand Identity**: Modern reinterpretation of Japanese culture
- **User Experience**: Intuitive navigation and attractive visuals
- **Conversion Optimization**: Lead generation with CTA buttons and subscription forms

## 🔮 Future Improvements

- [ ] Multi-language support (Japanese, English)
- [ ] Dark mode implementation
- [ ] Web accessibility enhancement (WCAG 2.1 compliance)
- [ ] PWA conversion
- [ ] Animation performance optimization

---

### 🤝 Contact

This project follows best practices in modern web development, pursuing clean code and scalable architecture.