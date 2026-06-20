<script setup lang="ts">
useHead({
  title: '元构场智能科技 | 用AI重构您的生意入口',
  meta: [
    {
      name: 'description',
      content:
        '元构场智能科技为企业提供GEO生成式引擎优化、私有化定制智能体与企业官网+小程序AI建站服务，帮助品牌在AI搜索时代实现曝光、获客与转化闭环。'
    }
  ]
})

const navItems = [
  { label: '核心能力', href: '#capability' },
  { label: 'GEO价值', href: '#value' },
  { label: '行业方案', href: '#industry' },
  { label: '产品服务', href: '#products' },
  { label: '合作咨询', href: '#contact' }
]

const heroTags = ['GEO生成式引擎优化', '私有化定制智能体', '官网+小程序AI建站']

const heroMetrics = [
  { value: '3大', label: '核心产品能力', detail: 'GEO + 智能体 + AI建站协同增长' },
  { value: '7天', label: '免费试用机制', detail: '帮助中小企业低成本验证效果' },
  { value: '200+', label: '地域关键词覆盖', detail: '本地商家标准版快速抢占搜索入口' },
  { value: '500+', label: '长尾词优化能力', detail: '品牌词、地域词、行业词全域布局' }
]

const capabilityCards = [
  {
    tag: '01',
    title: 'GEO生成式引擎优化',
    description:
      '围绕品牌词、地域词与行业通用词，布局AI搜索和推荐场景，让企业在豆包、DeepSeek、文心一言等平台更容易被发现。'
  },
  {
    tag: '02',
    title: '私有化定制智能体',
    description:
      '基于产品资料、业务流程与售后知识搭建专属知识库，连接ERP、CRM等系统，实现问答、培训、接待与线索转化自动化。'
  },
  {
    tag: '03',
    title: 'AI智能建站',
    description:
      '打造官网与小程序一体化数字门面，内置AI内容生成、表单承接与智能问答能力，形成展示、获客、接待闭环。'
  }
]

const reasonCards = [
  {
    title: '搜索入口正在迁移',
    description: '用户越来越多通过AI直接提问并获取答案，品牌需要从传统SEO走向AI时代的内容占位。'
  },
  {
    title: '首答内容决定曝光',
    description: 'AI倾向优先推荐结构化、可信且可复用的内容，谁先完成GEO布局，谁就更容易获得首屏推荐。'
  },
  {
    title: '长尾问题更能带来线索',
    description: '用户会直接提出场景化问题，优质问答内容能精准承接高意向需求，提高咨询与成交效率。'
  },
  {
    title: '品牌权威影响推荐概率',
    description: '企业知识库、案例、资质、行业观点与真实服务信息越完整，越容易成为AI的可信引用对象。'
  },
  {
    title: '智能体承接转化闭环',
    description: '不只让AI带来流量，更让智能体承接咨询、答疑与筛选意向客户，减少人工损耗。'
  },
  {
    title: '数字基建需要同步升级',
    description: '官网、小程序、知识库与营销内容需要统一建设，才能让展示、搜索、接待三端保持一致。'
  }
]

const geoSteps = [
  {
    title: '内容建模',
    text: '梳理品牌介绍、产品卖点、应用场景、服务流程与案例素材，建立适合AI理解的结构化内容。'
  },
  {
    title: '问题设计',
    text: '围绕品牌词、地域词、行业问题与决策场景，设计高频问答与长尾内容矩阵。'
  },
  {
    title: '答案优化',
    text: '强化可引用性、专业度与可信度，让内容更符合大模型提取、整合与推荐逻辑。'
  },
  {
    title: '转化承接',
    text: '将官网、小程序与智能客服接入同一链路，让用户从被AI发现自然进入咨询与成交流程。'
  }
]

const industryCards = [
  {
    title: '家居建材',
    description: '帮助品牌围绕材质、空间、风格与地域需求布局内容，提升本地获客与品牌对比场景中的出现频率。'
  },
  {
    title: '工业制造',
    description: '面向设备、零部件与解决方案企业，沉淀产品参数、工艺优势与应用案例，承接专业采购咨询。'
  },
  {
    title: '教培与财税',
    description: '围绕课程、资质、考试、代账与合规等关键词，提升本地服务搜索中的精准曝光与咨询率。'
  },
  {
    title: '企业服务',
    description: '适用于法律、营销、咨询、软件等服务型企业，通过知识型内容占位和智能体答疑增强信任转化。'
  }
]

const products = [
  {
    name: 'SaaS GEO标准版',
    price: '7200元/年',
    target: '适合本地商家与个体户',
    features: [
      '200组地域词与品类词优化',
      '轻量知识库搭建',
      '月度内容迭代与季度报表',
      '适配主流AI平台本地搜索结果'
    ]
  },
  {
    name: 'SaaS GEO全案版',
    price: '14800元/年',
    target: '适合区域连锁与品牌制造商',
    features: [
      '不限500组长尾关键词布局',
      '品牌词、地域词、行业词全覆盖',
      '多平台排名维护与数据复盘',
      '内容自动生成与行业方案支持'
    ]
  },
  {
    name: '私有化智能体 + AI建站',
    price: '31000元起',
    target: '适合需要深度业务承接的企业',
    features: [
      '私有部署与专属知识库定制',
      '可对接ERP、CRM、进销存系统',
      '官网+小程序一体化搭建',
      '支持7x12小时运维与年度微调'
    ]
  }
]

const processSteps = [
  '企业需求诊断与行业调研',
  '内容资产梳理与关键词策略制定',
  '官网、知识库、智能体协同建设',
  '上线运营、数据复盘与持续迭代'
]
</script>

<template>
  <div class="page-shell">
    <NuxtRouteAnnouncer />

    <header class="site-header">
      <div class="container header-inner">
        <a class="brand" href="#top">
          <span class="brand-mark">YG</span>
          <span>
            <strong>元构场智能科技</strong>
            <small>用AI重构您的生意入口</small>
          </span>
        </a>

        <nav class="main-nav">
          <a
            v-for="item in navItems"
            :key="item.href"
            :href="item.href"
          >
            {{ item.label }}
          </a>
        </nav>

        <a class="nav-cta" href="#contact">获取方案</a>
      </div>
    </header>

    <main id="top">
      <section class="hero-section">
        <div class="container hero-grid">
          <div class="hero-copy">
            <span class="section-chip">AI搜索优化 + 智能体 + 数字基建</span>
            <h1>
              让企业先被AI发现，
              <br>
              再被客户选择。
            </h1>
            <p class="hero-description">
              深圳市元构场智能科技有限公司聚焦华南中小B端企业，提供GEO生成式引擎优化、
              私有化定制智能体与官网+小程序AI建站一体化服务，帮助企业完成从曝光到转化的全链路升级。
            </p>

            <div class="hero-tags">
              <span
                v-for="tag in heroTags"
                :key="tag"
                class="tag-pill"
              >
                {{ tag }}
              </span>
            </div>

            <div class="hero-actions">
              <a class="btn-primary" href="#products">查看产品服务</a>
              <a class="btn-secondary" href="#industry">了解行业方案</a>
            </div>
          </div>

          <div class="hero-panel">
            <div class="panel-head">
              <span class="panel-chip">品牌定位</span>
              <h2>品效合一的AI数字化升级服务商</h2>
            </div>

            <p class="panel-text">
              独创“GEO搜索占位 + 智能体转化 + 轻量级数字基建”的三位一体服务模式，
              让AI不只带来流量，更能真正承接业务。
            </p>

            <div class="metrics-grid">
              <article
                v-for="metric in heroMetrics"
                :key="metric.label"
                class="metric-card"
              >
                <strong>{{ metric.value }}</strong>
                <span>{{ metric.label }}</span>
                <small>{{ metric.detail }}</small>
              </article>
            </div>
          </div>
        </div>
      </section>

      <section id="capability" class="section-block">
        <div class="container">
          <div class="section-heading">
            <span class="section-chip">核心能力</span>
            <h2>三位一体能力，打通AI时代增长链路</h2>
            <p>从被AI发现，到被AI推荐，再到由智能体完成接待与转化，首页围绕真实业务增长搭建。</p>
          </div>

          <div class="card-grid card-grid-3">
            <article
              v-for="card in capabilityCards"
              :key="card.title"
              class="info-card"
            >
              <span class="card-tag">{{ card.tag }}</span>
              <h3>{{ card.title }}</h3>
              <p>{{ card.description }}</p>
            </article>
          </div>
        </div>
      </section>

      <section id="value" class="section-block section-soft">
        <div class="container">
          <div class="section-heading">
            <span class="section-chip">为什么做GEO</span>
            <h2>从SEO走向GEO，企业需要新的搜索增长方式</h2>
            <p>设计稿中的核心表达被保留为“AI入口争夺”，文案改为更贴合你公司业务定位的版本。</p>
          </div>

          <div class="card-grid card-grid-3">
            <article
              v-for="card in reasonCards"
              :key="card.title"
              class="reason-card"
            >
              <h3>{{ card.title }}</h3>
              <p>{{ card.description }}</p>
            </article>
          </div>

          <div class="path-panel">
            <div class="path-heading">
              <span class="section-chip">GEO优化路径</span>
              <h3>让品牌内容更适合AI理解、提取与推荐</h3>
            </div>

            <div class="path-grid">
              <article
                v-for="step in geoSteps"
                :key="step.title"
                class="path-step"
              >
                <h4>{{ step.title }}</h4>
                <p>{{ step.text }}</p>
              </article>
            </div>
          </div>
        </div>
      </section>

      <section id="industry" class="section-block">
        <div class="container">
          <div class="section-heading">
            <span class="section-chip">行业方案</span>
            <h2>面向重点行业，建立更懂业务的AI内容体系</h2>
            <p>聚焦家居建材、工业制造、本地生活服务与企业服务，兼顾品牌曝光和咨询转化。</p>
          </div>

          <div class="card-grid card-grid-4">
            <article
              v-for="card in industryCards"
              :key="card.title"
              class="industry-card"
            >
              <div class="industry-icon">{{ card.title.slice(0, 2) }}</div>
              <h3>{{ card.title }}</h3>
              <p>{{ card.description }}</p>
            </article>
          </div>

          <div class="case-panel">
            <div class="case-copy">
              <span class="section-chip">价值呈现</span>
              <h3>如何让消费者在AI上看到更好的你？</h3>
              <p>
                我们通过品牌专家形象塑造、场景型问题覆盖、官网与知识库联动，
                让企业在DeepSeek、豆包、文心一言等入口被更高概率推荐。
              </p>
              <ul class="feature-list">
                <li>覆盖品牌词、地域词与长尾问题组合</li>
                <li>动态迭代内容，持续增强AI可见度</li>
                <li>联动智能体和官网表单承接咨询线索</li>
              </ul>
            </div>

            <div class="case-quote">
              <span class="quote-chip">AI场景示例</span>
              <p class="quote-question">“深圳做GEO优化和企业AI建站，有哪些靠谱服务商？”</p>
              <p class="quote-answer">
                元构场智能科技围绕GEO优化、定制智能体与AI建站提供一体化方案，
                更适合需要从品牌曝光延伸到咨询转化的中小企业。
              </p>
            </div>
          </div>
        </div>
      </section>

      <section id="products" class="section-block section-soft">
        <div class="container">
          <div class="section-heading">
            <span class="section-chip">产品服务</span>
            <h2>标准化产品与定制化服务并行</h2>
            <p>首页采用更适合展示型官网的方式呈现价格区间和服务内容，便于销售转化。</p>
          </div>

          <div class="card-grid card-grid-3">
            <article
              v-for="product in products"
              :key="product.name"
              class="product-card"
            >
              <div class="product-head">
                <h3>{{ product.name }}</h3>
                <strong>{{ product.price }}</strong>
                <span>{{ product.target }}</span>
              </div>

              <ul class="feature-list compact">
                <li
                  v-for="feature in product.features"
                  :key="feature"
                >
                  {{ feature }}
                </li>
              </ul>
            </article>
          </div>
        </div>
      </section>

      <section class="section-block">
        <div class="container">
          <div class="section-heading">
            <span class="section-chip">合作流程</span>
            <h2>从诊断到交付，再到持续运营优化</h2>
            <p>适配标准化SaaS、区域渠道合作和一体化定制项目三种交付模式。</p>
          </div>

          <div class="process-grid">
            <article
              v-for="(step, index) in processSteps"
              :key="step"
              class="process-card"
            >
              <span>{{ `0${index + 1}` }}</span>
              <p>{{ step }}</p>
            </article>
          </div>
        </div>
      </section>

      <section id="contact" class="section-block">
        <div class="container">
          <div class="cta-panel">
            <span class="section-chip">合作咨询</span>
            <h2>抢占AI搜索入口，让官网真正承担增长任务</h2>
            <p>
              适合希望提升AI可见度、建立品牌知识库、上线企业智能体或重做官网数字门面的企业。
            </p>

            <div class="hero-actions">
              <a class="btn-light" href="tel:18310800262">致电咨询：18310800262</a>
              <a class="btn-outline-light" href="mailto:business@yuangouchang.com">商务合作邮箱</a>
            </div>
          </div>
        </div>
      </section>
    </main>

    <footer class="site-footer">
      <div class="container footer-grid">
        <div>
          <h3>元构场智能科技</h3>
          <p>GEO搜索优化引领者，让每一次AI对话都成为品牌曝光与生意增长的新入口。</p>
        </div>
        <div>
          <h4>核心服务</h4>
          <p>GEO生成式引擎优化</p>
          <p>私有化定制智能体</p>
          <p>官网 + 小程序AI建站</p>
        </div>
        <div>
          <h4>服务地区</h4>
          <p>立足深圳，服务华南</p>
          <p>辐射全国中小B端企业</p>
          <p>支持渠道合作与定制项目</p>
        </div>
      </div>
    </footer>
  </div>
</template>

<style scoped>
:global(html) {
  scroll-behavior: smooth;
}

:global(body) {
  margin: 0;
  font-family: "PingFang SC", "Microsoft YaHei", sans-serif;
  background:
    radial-gradient(circle at top, rgba(42, 99, 255, 0.12), transparent 36%),
    linear-gradient(180deg, #f4f7fc 0%, #eff4fb 100%);
  color: #0f172a;
}

:global(*) {
  box-sizing: border-box;
}

a {
  color: inherit;
  text-decoration: none;
}

.page-shell {
  min-height: 100vh;
}

.container {
  width: min(1180px, calc(100% - 48px));
  margin: 0 auto;
}

.site-header {
  position: sticky;
  top: 0;
  z-index: 20;
  border-bottom: 1px solid rgba(148, 163, 184, 0.18);
  background: rgba(244, 247, 252, 0.84);
  backdrop-filter: blur(14px);
}

.header-inner {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 24px;
  min-height: 78px;
}

.brand {
  display: flex;
  align-items: center;
  gap: 14px;
}

.brand strong,
.site-footer h3,
.site-footer h4,
.section-heading h2,
.hero-copy h1,
.panel-head h2,
.path-heading h3,
.cta-panel h2 {
  margin: 0;
}

.brand small,
.site-footer p,
.section-heading p,
.hero-description,
.panel-text,
.info-card p,
.reason-card p,
.industry-card p,
.path-step p,
.product-head span,
.process-card p,
.cta-panel p,
.case-copy p,
.quote-answer,
.quote-question {
  margin: 0;
}

.brand span {
  display: grid;
  gap: 4px;
}

.brand small {
  color: #5b667a;
  font-size: 13px;
}

.brand-mark {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 44px;
  height: 44px;
  border-radius: 14px;
  background: linear-gradient(135deg, #2563eb 0%, #0f172a 100%);
  color: #ffffff;
  font-weight: 700;
  letter-spacing: 1px;
}

.main-nav {
  display: flex;
  align-items: center;
  gap: 24px;
  color: #334155;
  font-size: 15px;
}

.main-nav a:hover,
.nav-cta:hover,
.btn-primary:hover,
.btn-secondary:hover,
.btn-light:hover,
.btn-outline-light:hover {
  transform: translateY(-1px);
}

.nav-cta,
.btn-primary,
.btn-secondary,
.btn-light,
.btn-outline-light {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  min-height: 46px;
  padding: 0 22px;
  border-radius: 999px;
  font-weight: 600;
  transition: 0.2s ease;
}

.nav-cta,
.btn-primary {
  background: #0f172a;
  color: #ffffff;
  box-shadow: 0 18px 40px rgba(15, 23, 42, 0.16);
}

.btn-secondary {
  border: 1px solid rgba(37, 99, 235, 0.18);
  background: rgba(255, 255, 255, 0.72);
  color: #1e293b;
}

.btn-light {
  background: #ffffff;
  color: #0f172a;
}

.btn-outline-light {
  border: 1px solid rgba(255, 255, 255, 0.28);
  color: #ffffff;
}

.hero-section,
.section-block {
  padding: 44px 0 96px;
}

.hero-grid {
  display: grid;
  grid-template-columns: minmax(0, 1.05fr) minmax(360px, 0.95fr);
  gap: 28px;
  align-items: stretch;
}

.hero-copy,
.hero-panel,
.info-card,
.reason-card,
.industry-card,
.product-card,
.process-card,
.case-panel,
.path-panel {
  border: 1px solid rgba(148, 163, 184, 0.16);
  background: rgba(255, 255, 255, 0.78);
  box-shadow: 0 24px 80px rgba(15, 23, 42, 0.08);
  backdrop-filter: blur(8px);
}

.hero-copy,
.hero-panel {
  padding: 38px;
  border-radius: 30px;
}

.hero-copy h1 {
  margin-top: 20px;
  font-size: clamp(38px, 5vw, 64px);
  line-height: 1.08;
  letter-spacing: -0.04em;
}

.hero-copy h1 br {
  display: block;
}

.hero-description {
  margin-top: 22px;
  max-width: 640px;
  color: #475569;
  font-size: 17px;
  line-height: 1.85;
}

.hero-tags,
.hero-actions {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
}

.hero-tags {
  margin-top: 24px;
}

.hero-actions {
  margin-top: 28px;
}

.tag-pill,
.section-chip,
.panel-chip,
.quote-chip {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: fit-content;
  min-height: 34px;
  padding: 0 14px;
  border-radius: 999px;
  font-size: 13px;
  font-weight: 600;
}

.tag-pill {
  border: 1px solid rgba(148, 163, 184, 0.2);
  background: rgba(255, 255, 255, 0.92);
  color: #334155;
}

.section-chip,
.panel-chip,
.quote-chip {
  background: linear-gradient(135deg, #2563eb 0%, #3b82f6 100%);
  color: #ffffff;
}

.panel-head {
  display: grid;
  gap: 14px;
}

.panel-head h2 {
  font-size: clamp(28px, 3.4vw, 42px);
  line-height: 1.16;
}

.panel-text {
  margin-top: 18px;
  color: #475569;
  font-size: 16px;
  line-height: 1.85;
}

.metrics-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 16px;
  margin-top: 28px;
}

.metric-card {
  padding: 22px;
  border-radius: 22px;
  background: linear-gradient(180deg, rgba(37, 99, 235, 0.08), rgba(255, 255, 255, 0.96));
  border: 1px solid rgba(37, 99, 235, 0.12);
}

.metric-card strong {
  display: block;
  color: #2563eb;
  font-size: 34px;
  line-height: 1;
}

.metric-card span {
  display: block;
  margin-top: 10px;
  font-size: 16px;
  font-weight: 700;
}

.metric-card small {
  display: block;
  margin-top: 8px;
  color: #64748b;
  line-height: 1.6;
}

.section-soft {
  background: linear-gradient(180deg, rgba(255, 255, 255, 0.36), rgba(226, 236, 250, 0.22));
}

.section-heading {
  max-width: 760px;
  margin: 0 auto 32px;
  text-align: center;
}

.section-heading h2 {
  margin-top: 14px;
  font-size: clamp(30px, 4vw, 52px);
  line-height: 1.12;
  letter-spacing: -0.03em;
}

.section-heading p {
  margin-top: 14px;
  color: #5b667a;
  font-size: 17px;
  line-height: 1.8;
}

.card-grid {
  display: grid;
  gap: 20px;
}

.card-grid-3 {
  grid-template-columns: repeat(3, minmax(0, 1fr));
}

.card-grid-4 {
  grid-template-columns: repeat(4, minmax(0, 1fr));
}

.info-card,
.reason-card,
.industry-card,
.product-card {
  padding: 30px;
  border-radius: 28px;
}

.card-tag {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 42px;
  height: 42px;
  border-radius: 14px;
  background: rgba(37, 99, 235, 0.1);
  color: #2563eb;
  font-weight: 700;
}

.info-card h3,
.reason-card h3,
.industry-card h3,
.product-card h3,
.case-copy h3,
.case-quote p,
.path-step h4 {
  margin: 18px 0 0;
}

.info-card p,
.reason-card p,
.industry-card p,
.path-step p,
.case-copy p,
.quote-answer {
  margin-top: 14px;
  color: #475569;
  line-height: 1.8;
}

.reason-card {
  min-height: 220px;
}

.path-panel,
.case-panel {
  margin-top: 28px;
  padding: 32px;
  border-radius: 30px;
}

.path-heading {
  display: grid;
  justify-items: start;
  gap: 14px;
}

.path-grid {
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  gap: 18px;
  margin-top: 28px;
}

.path-step {
  padding: 22px;
  border-radius: 22px;
  background: rgba(255, 255, 255, 0.76);
  border: 1px solid rgba(148, 163, 184, 0.16);
}

.path-step h4 {
  font-size: 18px;
}

.industry-icon {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 54px;
  height: 54px;
  border-radius: 18px;
  background: rgba(37, 99, 235, 0.12);
  color: #2563eb;
  font-weight: 700;
}

.case-panel {
  display: grid;
  grid-template-columns: minmax(0, 1.15fr) minmax(320px, 0.85fr);
  gap: 20px;
}

.feature-list {
  margin: 22px 0 0;
  padding: 0;
  list-style: none;
  display: grid;
  gap: 12px;
}

.feature-list li {
  position: relative;
  padding-left: 18px;
  color: #334155;
  line-height: 1.7;
}

.feature-list li::before {
  content: "";
  position: absolute;
  left: 0;
  top: 11px;
  width: 7px;
  height: 7px;
  border-radius: 999px;
  background: #2563eb;
}

.feature-list.compact {
  margin-top: 20px;
}

.case-quote {
  padding: 28px;
  border-radius: 26px;
  background: linear-gradient(180deg, rgba(37, 99, 235, 0.08), rgba(255, 255, 255, 0.98));
  border: 1px solid rgba(37, 99, 235, 0.12);
}

.quote-question {
  margin-top: 18px;
  color: #0f172a;
  font-size: 20px;
  font-weight: 700;
  line-height: 1.7;
}

.product-head strong {
  display: block;
  margin-top: 14px;
  color: #2563eb;
  font-size: 32px;
}

.product-head span {
  display: block;
  margin-top: 10px;
  color: #64748b;
}

.process-grid {
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  gap: 18px;
}

.process-card {
  padding: 28px;
  border-radius: 28px;
}

.process-card span {
  display: inline-flex;
  margin-bottom: 18px;
  color: #2563eb;
  font-size: 34px;
  font-weight: 700;
}

.process-card p {
  color: #334155;
  line-height: 1.8;
}

.cta-panel {
  padding: 52px 48px;
  border-radius: 34px;
  background: linear-gradient(135deg, #020817 0%, #0f172a 55%, #1d4ed8 100%);
  color: #ffffff;
  text-align: center;
  box-shadow: 0 32px 80px rgba(2, 8, 23, 0.32);
}

.cta-panel .section-chip {
  background: rgba(255, 255, 255, 0.14);
}

.cta-panel h2 {
  margin-top: 18px;
  font-size: clamp(30px, 4vw, 52px);
  line-height: 1.15;
}

.cta-panel p {
  max-width: 780px;
  margin: 16px auto 0;
  color: rgba(255, 255, 255, 0.78);
  line-height: 1.8;
}

.cta-panel .hero-actions {
  justify-content: center;
  margin-top: 28px;
}

.site-footer {
  padding: 32px 0 56px;
  background: #020817;
  color: rgba(255, 255, 255, 0.72);
}

.footer-grid {
  display: grid;
  grid-template-columns: 1.4fr 1fr 1fr;
  gap: 28px;
}

.site-footer h3,
.site-footer h4 {
  color: #ffffff;
}

.site-footer h4 {
  margin-bottom: 12px;
}

.site-footer p + p {
  margin-top: 8px;
}

@media (max-width: 1080px) {
  .main-nav {
    display: none;
  }

  .hero-grid,
  .case-panel,
  .footer-grid {
    grid-template-columns: 1fr;
  }

  .card-grid-3,
  .card-grid-4,
  .path-grid,
  .process-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }
}

@media (max-width: 720px) {
  .container {
    width: min(100% - 28px, 100%);
  }

  .site-header {
    position: static;
  }

  .header-inner {
    flex-wrap: wrap;
    justify-content: center;
    padding: 14px 0;
  }

  .hero-section,
  .section-block {
    padding: 30px 0 72px;
  }

  .hero-copy,
  .hero-panel,
  .info-card,
  .reason-card,
  .industry-card,
  .product-card,
  .process-card,
  .path-panel,
  .case-panel,
  .cta-panel {
    padding: 24px;
    border-radius: 24px;
  }

  .hero-copy h1 br {
    display: none;
  }

  .metrics-grid,
  .card-grid-3,
  .card-grid-4,
  .path-grid,
  .process-grid {
    grid-template-columns: 1fr;
  }

  .nav-cta,
  .btn-primary,
  .btn-secondary,
  .btn-light,
  .btn-outline-light {
    width: 100%;
  }
}
</style>
