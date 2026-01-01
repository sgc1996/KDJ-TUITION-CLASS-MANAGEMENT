<template>
  <q-page class="bg-black text-white font-inter">
    
    <!-- Navbar -->
    <header class="q-py-md fixed-top bg-black-translucent blur-md z-max border-bottom-dark transition-all">
      <div class="container-xl q-mx-auto row justify-between items-center q-px-md">
        <!-- Logo -->
        <div class="row items-center cursor-pointer">
          <div class="bg-primary text-white rounded-borders q-pa-xs q-mr-sm flex flex-center shadow-glow" style="width: 40px; height: 40px">
            <q-icon name="school" size="24px" />
          </div>
          <div class="text-h6 text-weight-900 tracking-tight leading-none text-white flex items-center">
            KDJ <span class="text-weight-300 text-caption text-uppercase tracking-widest text-grey-5 q-ml-sm">Tuition</span>
          </div>
        </div>

        <nav class="gt-sm row items-center q-gutter-sm">
          <q-btn flat class="nav-btn text-grey-4" label="Features" no-caps />
          <q-btn flat class="nav-btn text-grey-4" label="How it Works" no-caps />
          <q-btn flat class="nav-btn text-grey-4" label="Reviews" no-caps />
          <div class="vertical-separator q-mx-sm bg-grey-8" style="height: 24px"></div>
          <q-btn unelevated color="white" text-color="black" label="Login" no-caps class="q-px-lg rounded-lg shadow-white-glow" />
        </nav>
        <q-btn flat round icon="menu" color="white" class="lt-md" />
      </div>
    </header>

    <!-- Hero Section (Full Width Background) -->
    <section class="min-h-screen flex items-center relative-position overflow-hidden q-pt-xl q-pb-xl">
      <!-- Background Image -->
      <q-img 
        src="~assets/hero_bg_dark.png" 
        class="absolute-full" 
        style="z-index: 0; opacity: 0.6;" 
        fit="cover"
      />
      <!-- Gradient Overlay -->
      <div class="absolute-full bg-gradient-overlay" style="z-index: 1;"></div>

      <div class="container-xl q-mx-auto row items-center q-px-md relative-position" style="z-index: 2; padding-top: 80px;">
        <div class="col-12 col-md-7 q-pr-md-xl q-mb-xl q-mb-md-none" data-aos="fade-up">
          
          <div class="row items-center q-mb-lg">
             <q-badge color="grey-9" text-color="white" class="q-px-sm q-py-xs rounded-full border-grey-8">
               <q-icon name="rocket_launch" color="primary" size="14px" class="q-mr-xs" />
               v2.0 Beta Release
             </q-badge>
          </div>

          <h1 class="text-display text-weight-900 leading-tight q-mt-none q-mb-lg text-white text-shadow-lg">
            Manage your class <br />
            like a <span class="text-gradient-primary">Pro.</span>
          </h1>
          
          <p class="text-h6 text-grey-4 q-mb-xl text-weight-regular" style="max-width: 600px; line-height: 1.6;">
            The all-in-one tuition management platform designed for the modern era. 
            Seamlessly integrate students, payments, and attendance in one beautiful dashboard.
          </p>
          
          <div class="row q-gutter-md">
            <q-btn unelevated color="primary" size="lg" label="Get Started Free" icon-right="arrow_forward" no-caps class="q-px-xl q-py-md rounded-lg shadow-primary-lg transition-transform" />
            <q-btn outline color="white" size="lg" label="View Demo" icon="play_circle" no-caps class="q-px-xl q-py-md rounded-lg hover-bg-white-10" />
          </div>
          
          <div class="q-mt-xl row items-center q-gutter-x-lg text-grey-5">
             <div class="row items-center q-gutter-sm">
               <q-rate v-model="rating" size="18px" color="warning" readonly />
               <span class="text-weight-bold text-white">4.9/5</span>
               <span class="text-caption">User Rating</span>
             </div>
             <div class="vertical-separator bg-grey-8"></div>
             <div class="row items-center">
                <q-icon name="groups" class="q-mr-sm" size="20px" />
                <span class="text-weight-medium">Trusted by 500+ Tutors</span>
             </div>
          </div>
        </div>
        
        <!-- Hero Right Side (Glass Card) -->
        <div class="col-12 col-md-5 relative-position">
            <q-card class="glass-panel-dark q-pa-lg animate-float border-white-10 shadow-2xl">
               <div class="row items-center justify-between q-mb-lg">
                 <div>
                   <div class="text-subtitle2 text-grey-4">Total Revenue</div>
                   <div class="text-h4 text-weight-bold">LKR 450,000</div>
                 </div>
                 <q-avatar color="primary" icon="attach_money" />
               </div>
               
               <!-- Fake Chart Bars -->
               <div class="row items-end justify-between q-mb-md" style="height: 100px">
                  <div class="bg-primary rounded-t-sm" style="width: 12%; height: 40%; opacity: 0.5"></div>
                  <div class="bg-primary rounded-t-sm" style="width: 12%; height: 60%; opacity: 0.7"></div>
                  <div class="bg-primary rounded-t-sm" style="width: 12%; height: 30%; opacity: 0.4"></div>
                  <div class="bg-primary rounded-t-sm" style="width: 12%; height: 80%; opacity: 0.9"></div>
                  <div class="bg-primary rounded-t-sm" style="width: 12%; height: 60%; opacity: 0.6"></div>
                  <div class="bg-primary rounded-t-sm shadow-glow-bar" style="width: 12%; height: 100%;"></div>
               </div>
               
               <div class="text-caption text-grey-5 text-center">Revenue Analytics (Last 6 Months)</div>
               
               <q-separator color="grey-8" class="q-my-md" />
               
               <div class="row items-center">
                  <q-icon name="trending_up" color="green-4" class="q-mr-sm" />
                  <span class="text-green-4 text-weight-bold">+24%</span>
                  <span class="q-ml-sm text-grey-5">increase vs last month</span>
               </div>
            </q-card>
        </div>
      </div>
    </section>

    <!-- Logo Cloud -->
    <section class="q-py-lg bg-black border-y-dark">
      <div class="container-xl q-mx-auto text-center">
        <p class="text-caption text-uppercase tracking-widest text-grey-7 q-mb-lg text-weight-bold">Trusted by top education institutes</p>
        <div class="flex flex-center q-gutter-xl opacity-30 grayscale hover-grayscale-off transition-all">
           <div class="row items-center text-h5 text-white text-weight-bold"><q-icon name="school" class="q-mr-sm" />EduSmart</div>
           <div class="row items-center text-h5 text-white text-weight-bold"><q-icon name="menu_book" class="q-mr-sm" />ClassMate</div>
           <div class="row items-center text-h5 text-white text-weight-bold"><q-icon name="psychology" class="q-mr-sm" />TutorPro</div>
           <div class="row items-center text-h5 text-white text-weight-bold"><q-icon name="auto_stories" class="q-mr-sm" />NextGen</div>
        </div>
      </div>
    </section>

    <!-- Value Proposition / Features Grid -->
    <section class="q-py-xl q-my-xl">
      <div class="container-xl q-mx-auto q-pa-md">
        <div class="text-center q-mb-xl" data-aos="fade-up">
          <q-chip color="grey-9" text-color="primary" icon="bolt" label="Fast & efficient" size="md" class="border-grey-8" />
          <h2 class="text-h3 text-weight-900 q-mb-md q-mt-md text-white">Everything you need to <br/> run your class.</h2>
          <p class="text-grey-5 text-h6 text-weight-regular">Powerful features without the complexity.</p>
        </div>

        <div class="row q-col-gutter-lg">
          <div class="col-12 col-md-4" v-for="(feature, i) in features" :key="i">
            <q-card flat class="h-full feature-card-dark q-pa-lg rounded-xl bg-grey-10 border-white-5">
              <div class="bg-grey-9 q-pa-md inline-block rounded-lg q-mb-lg icon-box-dark">
                 <q-icon :name="feature.icon" size="32px" color="primary" />
              </div>
              <div class="text-h5 text-weight-bold q-mb-sm text-white">{{ feature.title }}</div>
              <div class="text-grey-5 text-body1 leading-relaxed">{{ feature.desc }}</div>
            </q-card>
          </div>
        </div>
      </div>
    </section>

    <!-- Detailed Feature 1 -->
    <section class="q-py-xl overflow-hidden bg-gradient-dark text-white section-dots-pattern">
      <div class="container-xl q-mx-auto q-pa-md">
        <div class="row items-center q-col-gutter-xl">
          <div class="col-12 col-md-6 order-last order-md-first">
             <div class="relative-position">
                <div class="absolute-inset bg-primary blur-2xl opacity-20 rounded-full"></div>
                <q-img src="~assets/dashboard_analytics.png" class="rounded-xl shadow-glow-blue hover-scale relative-position z-10 border-white-10" />
             </div>
          </div>
          <div class="col-12 col-md-6 q-pl-md-xl">
            <div class="text-primary text-subtitle2 text-uppercase text-weight-bolder q-mb-sm tracking-widest">Analytics</div>
            <h3 class="text-h3 text-weight-bold q-mb-md">Data-driven decisions <br/>at your fingertips.</h3>
            <p class="text-grey-5 text-h6 text-weight-regular q-mb-lg">
              Visualise your class performance with our advanced analytics dashboard. Track student progress, payments, and attendance trends in real-time.
            </p>
            <q-list dark padding separator>
              <q-item v-for="n in 3" :key="n" class="q-px-none border-grey-8">
                <q-item-section avatar><q-icon name="check_circle" color="primary" /></q-item-section>
                <q-item-section class="text-h6 text-weight-light">Real-time revenue tracking</q-item-section>
              </q-item>
            </q-list>
          </div>
        </div>
      </div>
    </section>

    <!-- Detailed Feature 2 -->
    <section class="q-py-xl q-my-xl">
      <div class="container-xl q-mx-auto q-pa-md">
        <div class="row items-center q-col-gutter-xl">
          <div class="col-12 col-md-6 q-pr-md-xl">
            <div class="text-accent text-subtitle2 text-uppercase text-weight-bolder q-mb-sm tracking-widest">Mobile App</div>
            <h3 class="text-h3 text-weight-900 q-mb-md text-white">Attendance in <br/>your pocket.</h3>
            <p class="text-grey-5 text-h6 text-weight-regular q-mb-xl">
              Say goodbye to paper registers. Use our dedicated mobile app to scan QR codes and mark attendance instantly.
            </p>
            
            <div class="row q-gutter-xl q-mb-xl">
               <div>
                 <h3 class="q-my-none text-weight-900 text-white">0.5s</h3>
                 <div class="text-body2 text-uppercase text-weight-bold text-grey-7">Scan Time</div>
               </div>
               <div class="vertical-separator bg-grey-8"></div>
               <div>
                 <h3 class="q-my-none text-weight-900 text-white">100%</h3>
                 <div class="text-body2 text-uppercase text-weight-bold text-grey-7">Accuracy</div>
               </div>
            </div>
            
            <q-btn unelevated color="white" text-color="black" label="Download App" icon="system_update" class="q-py-sm q-px-lg rounded-lg shadow-white-glow" />
          </div>
          <div class="col-12 col-md-6 text-center relative-position">
              <div class="blob-bg-2 absolute-center opacity-30"></div>
             <q-img src="~assets/mobile_app.png" style="max-width: 320px;" class="rounded-xl shadow-glow-accent hover-lift-lg inline-block relative-position z-10 border-white-10" />
          </div>
        </div>
      </div>
    </section>

     <!-- CTA Section -->
    <section class="q-py-xl relative-position overflow-hidden">
       <!-- Dynamic Background for CTA -->
      <div class="absolute-full bg-gradient-primary"></div>
      
      <div class="container-sm q-mx-auto text-center relative-position z-10 q-pa-xl">
        <h2 class="text-h2 text-weight-900 q-mb-lg text-white">Ready to transform your class?</h2>
        <p class="text-h6 text-white-80 q-mb-xl text-weight-light">Join hundreds of other tuition masters who switched to KDJ Tuition v2.</p>
        <q-btn color="white" text-color="primary" size="xl" label="Start your Free Trial" no-caps class="q-px-xl rounded-lg shadow-2xl" />
        <div class="q-mt-md text-white-60 text-caption">No credit card required • Cancel anytime</div>
      </div>
    </section>

    <!-- Footer -->
    <footer class="bg-black q-py-xl border-top-dark">
      <div class="container-xl q-mx-auto q-pa-md">
        <div class="row q-col-gutter-xl">
          <div class="col-12 col-md-4">
             <div class="row items-center q-mb-md">
                <div class="bg-primary text-white rounded-borders q-pa-xs q-mr-sm flex flex-center" style="width: 32px; height: 32px">
                    <q-icon name="school" size="18px" />
                </div>
                <span class="text-h6 text-weight-bold text-white">KDJTUITION</span>
             </div>
             <p class="text-grey-6 leading-relaxed">Empowering education through technology. The most advanced class management system designed for tutors.</p>
             <div class="row q-gutter-sm q-mt-md">
                <q-btn round flat size="sm" icon="facebook" color="grey-6" />
                <q-btn round flat size="sm" icon="smart_display" color="grey-6" />
                <q-btn round flat size="sm" icon="check_circle" color="grey-6" />
             </div>
          </div>
          <div class="col-6 col-md-2 offset-md-2">
            <div class="text-subtitle2 text-weight-bold q-mb-md text-uppercase text-grey-6">Product</div>
            <div class="flex column q-gutter-sm text-grey-5">
              <a href="#" class="footer-link">Features</a>
              <a href="#" class="footer-link">Pricing</a>
              <a href="#" class="footer-link">Updates</a>
            </div>
          </div>
           <div class="col-6 col-md-2">
            <div class="text-subtitle2 text-weight-bold q-mb-md text-uppercase text-grey-6">Company</div>
            <div class="flex column q-gutter-sm text-grey-5">
              <a href="#" class="footer-link">About</a>
              <a href="#" class="footer-link">Careers</a>
              <a href="#" class="footer-link">Contact</a>
            </div>
          </div>
           <div class="col-6 col-md-2">
            <div class="text-subtitle2 text-weight-bold q-mb-md text-uppercase text-grey-6">Legal</div>
            <div class="flex column q-gutter-sm text-grey-5">
              <a href="#" class="footer-link">Privacy</a>
              <a href="#" class="footer-link">Terms</a>
            </div>
          </div>
        </div>
        <div class="q-mt-xl text-center text-grey-8 border-top-dark q-pt-lg text-caption">
          &copy; 2026 KDJ Tuition Management. All rights reserved.
        </div>
      </div>
    </footer>

  </q-page>
</template>

<script setup>
import { ref } from 'vue'

const rating = ref(4.9)

const features = [
  {
    icon: 'school',
    title: 'Student Profiles',
    desc: '360-degree view of every student. Academic history, payment records, and personal notes in one place.'
  },
  {
    icon: 'qr_code_2',
    title: 'Smart Attendance',
    desc: 'Lightning fast QR check-ins. Auto SMS notifications to parents when a student enters or leaves.'
  },
  {
    icon: 'payments',
    title: 'Fee Management',
    desc: 'Automated monthly fee generation. Partial payments, arrears tracking, and printed receipts.'
  },
  {
    icon: 'analytics',
    title: 'Deep Analytics',
    desc: 'Understand your growth with revenue charts, student retention graphs, and subject popularity.'
  },
   {
    icon: 'notifications_active',
    title: 'SMS Alerts',
    desc: 'Keep parents informed with automated SMS for attendance, payments, and class cancellations.'
  },
   {
    icon: 'lock',
    title: 'Secure & Safe',
    desc: 'Enterprise grade security for your data. Daily backups and role-based access control.'
  }
]
</script>

<style lang="scss" scoped>
/* Typography & Utilities */
.font-inter {
  font-family: 'Inter', -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
}
.text-display {
  font-size: 4rem;
  letter-spacing: -0.02em;
  @media (max-width: 600px) {
    font-size: 2.75rem;
  }
}
.leading-tight { line-height: 1.1; }
.leading-relaxed { line-height: 1.6; }
.tracking-tight { letter-spacing: -0.02em; }
.tracking-widest { letter-spacing: 0.15em; }

/* Colors & Gradients */
.text-gradient-primary {
  background: linear-gradient(135deg, #2979ff 0%, #00e676 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
.bg-gradient-overlay {
    background: linear-gradient(180deg, rgba(0,0,0,0.85) 0%, rgba(0,0,0,0.95) 100%);
}
.bg-gradient-primary {
    background: linear-gradient(135deg, #0d47a1 0%, #1565c0 100%);
}
.bg-gradient-dark {
    background: linear-gradient(to bottom, #000000, #0a0a0a);
}
.bg-black-translucent {
  background: rgba(0, 0, 0, 0.7);
}
.text-white-80 { color: rgba(255,255,255,0.8); }
.text-white-60 { color: rgba(255,255,255,0.6); }

/* Layout */
.container-xl { max-width: 1200px; }
.container-sm { max-width: 800px; }
.min-h-screen { min-height: 100vh; }

/* Components */
.nav-btn {
    font-weight: 500;
    font-size: 15px;
    &:hover {
        background: transparent;
        color: #fff !important;
    }
}
.footer-link {
    text-decoration: none;
    color: inherit;
    transition: color 0.2s;
    &:hover {
        color: #2979ff;
    }
}
.rounded-t-sm { border-top-left-radius: 4px; border-top-right-radius: 4px; }
.rounded-xl { border-radius: 16px; }
.rounded-lg { border-radius: 10px; }
.rounded-full { border-radius: 9999px; }

/* Effects and Shadows */
.blur-md { backdrop-filter: blur(12px); }
.blur-2xl { filter: blur(40px); }
.shadow-glow { box-shadow: 0 0 15px rgba(41, 121, 255, 0.5); }
.shadow-glow-bar { box-shadow: 0 0 10px rgba(41, 121, 255, 0.8); }
.shadow-glow-blue { box-shadow: 0 20px 50px -10px rgba(41, 121, 255, 0.3); }
.shadow-glow-accent { box-shadow: 0 20px 50px -10px rgba(0, 230, 118, 0.2); }
.shadow-primary-lg { box-shadow: 0 10px 30px rgba(41, 121, 255, 0.4); }
.shadow-white-glow { box-shadow: 0 0 15px rgba(255,255,255,0.3); }

/* Interactions */
.feature-card-dark {
  transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
  border: 1px solid rgba(255,255,255,0.05);
  &:hover {
    border-color: #2979ff;
    transform: translateY(-5px);
    background: #111;
    .icon-box-dark {
        background-color: #2979ff;
        .q-icon { color: white !important; }
    }
  }
}
.hover-lift-lg:hover { transform: translateY(-10px); transition: transform 0.4s ease; }
.hover-bg-white-10:hover { background: rgba(255,255,255,0.1); }
.hover-grayscale-off:hover { filter: grayscale(0); opacity: 1; }
.grayscale { filter: grayscale(100%); }

/* Backgrounds & Decorations */
.border-grey-8 { border: 1px solid #424242; }
.border-dark { border-top: 1px solid #212121; border-bottom: 1px solid #212121; }
.border-top-dark { border-top: 1px solid #212121; }
.border-white-10 { border: 1px solid rgba(255,255,255,0.1); border-left: 1px solid rgba(255,255,255,0.2); }
.border-white-5 { border: 1px solid rgba(255,255,255,0.05); }

.glass-panel-dark {
  background: rgba(20, 20, 20, 0.7);
  backdrop-filter: blur(16px);
  border-radius: 16px;
}
.text-shadow-lg { text-shadow: 0 4px 10px rgba(0,0,0,0.5); }

.blob-bg-2 {
    width: 300px; height: 300px;
    background: radial-gradient(circle, rgba(41,121,255,0.2) 0%, rgba(0,0,0,0) 70%);
}

.animate-float { animation: float 6s ease-in-out infinite; }
@keyframes float {
    0% { transform: translateY(0px); }
    50% { transform: translateY(-10px); }
    100% { transform: translateY(0px); }
}

.z-max { z-index: 1000; }
</style>
