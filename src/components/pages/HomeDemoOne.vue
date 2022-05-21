<template>
    <div>
        <Navbar />
        <MainBanner />
        <Featured />
        <Experience />
        <Services />
        <!-- <ServicesTwo />
        <ServicesThree /> -->
        <!-- <Comparisons /> -->
             <SectionProject />
        <Sectiondeals />
        <!-- <FeaturesTwo /> -->
        <Invoicing />
        <!-- <FunFacts /> -->
        <!-- <Feedback /> -->
        <!-- <ReadyToTalk /> -->
        <Partner />
        <AppDownload />
        <Subscribe />
   

        <!-- <AccountCreate /> -->
        <Footer />
    </div>
</template>

<script>
import Navbar from '../layout/Navbar'
import MainBanner from '../home-demo-four/MainBanner'
import Featured from '../common/Featured'
import Experience from '../home-demo-four/Experience'
import Services from '../common/Services'
// import ServicesTwo from '../common/ServicesTwo'
// import ServicesThree from '../common/ServicesThree'
// import Comparisons from '../common/Comparisons'
import SectionProject from '../home-demo-one/SectionProject'
import Sectiondeals from '../home-demo-one/Sectiondeals'
// import FeaturesTwo from '../common/FeaturesTwo'
import Invoicing from '../common/Invoicing'
// import FunFacts from '../common/FunFacts'
// import Feedback from '../common/Feedback'
// import ReadyToTalk from '../common/ReadyToTalk'
import Partner from '../common/Partner'
import AppDownload from '../common/AppDownload'
import Subscribe from '../home-demo-six/Subscribe'

// import AccountCreate from '../common/AccountCreate'
import Footer from '../layout/Footer'

export default {
    name: 'HomeDemoOne',
    components: {
        Navbar,
        MainBanner,
        Featured,
        Experience,
        Services,
        // ServicesTwo,
        // ServicesThree,
        // Comparisons,

        SectionProject,
           Sectiondeals,
        // FeaturesTwo,
        Invoicing,
        // FunFacts,
        // Feedback,
        // ReadyToTalk,
        Partner,
        AppDownload,
           Subscribe,
           
        // AccountCreate,
        Footer,
    }
}
</script>
