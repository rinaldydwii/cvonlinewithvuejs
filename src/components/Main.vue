<template>
  <main>
    <div class="container">
      <app-profile :sectionData="profile"></app-profile>
      <app-section :sectionData="education"></app-section>
      <app-section :sectionData="organization"></app-section>
      <app-section :sectionData="work"></app-section>
      <app-section :sectionData="skill"></app-section>
      <app-section :sectionData="interest"></app-section>
      <app-section :sectionData="portfolio"></app-section>
      <app-section :sectionData="socialMedia"></app-section>
      <hr />
    </div>
  </main>
</template>

<script>
import Profile from './Profile'
import Section from './Section'

export default {
  name: 'Main',
  components: {
    'app-profile': Profile,
    'app-section': Section
  },
  data () {
    return {
      profile: {
        title: '• Profile •',
        birth: 'Jambi, January 16th, 1995',
        address1: 'Jl. Galur Sari Timur Gg. Urunsari RT013/RW01 No.1',
        address2: 'Utan Kayu Selatan, Matraman, Jakarta Timur - 13120'
      },
      education: {
        title: '• Education •',
        class: 'education',
        item: [
          { id: '1',
            year: '2010 - 2013',
            mainContent: 'SMA Negeri 1 Kuta Utara',
            subContent: ''
          },
          { id: '2',
            year: '2013 - 2017',
            mainContent: 'Telkom University',
            subContent: 'Bachelor of Informatics Engineering'
          }
        ]
      },
      organization: {
        title: '• Organization Experience •',
        class: 'organization',
        item: [
          { id: '1',
            year: 'Jan 2015 - Jan 2016',
            mainContent: 'Project Laboratory Assistant',
            subContent: 'Multimedia Laboratory Telkom University'
          },
          { id: '2',
            year: 'Jan 2016 - Feb 2017',
            mainContent: 'Coordinator of Laboratory Assistant',
            subContent: 'Multimedia Laboratory Telkom University'
          }
        ]
      },
      work: {
        title: '• Work Experience •',
        class: 'work',
        item: [
          { id: '1',
            year: 'Jun - Aug 2016',
            mainContent: 'PT. Garuda Maintenance Facility (GMF) AeroAsia',
            subContent: 'Internship'
          },
          { id: '2',
            year: 'Dec 2017 - NOW',
            mainContent: 'PT. Media Sport Indonesia (indosport.com)',
            subContent: 'Front End Programmer'
          }
        ]
      },
      skill: {
        title: '• Skill •',
        class: 'skill',
        item: [
          { id: '1',
            icon: '/static/html.svg',
            name: 'HTML',
            rate: 4
          },
          { id: '2',
            icon: '/static/css.svg',
            name: 'CSS',
            rate: 4
          },
          { id: '3',
            icon: '/static/php.svg',
            name: 'PHP',
            rate: 3
          },
          { id: '4',
            icon: '/static/javascript.svg',
            name: 'Javascript',
            rate: 3
          },
          { id: '5',
            icon: '/static/jquery.svg',
            name: 'JQuery',
            rate: 3
          },
          { id: '6',
            icon: '/static/laravel.svg',
            name: 'Laravel',
            rate: 3
          },
          { id: '7',
            icon: '/static/mysql.svg',
            name: 'MySQL',
            rate: 3
          },
          { id: '8',
            icon: '/static/mongodb.svg',
            name: 'MongoDB',
            rate: 2
          },
          { id: '9',
            icon: '/static/reactjs.svg',
            name: 'ReactJS',
            rate: 3
          },
          { id: '10',
            icon: '/static/nodejs.svg',
            name: 'NodeJS',
            rate: 2
          },
          { id: '11',
            icon: '/static/git.svg',
            name: 'Git',
            rate: 2
          },
          { id: '12',
            icon: '/static/photoshop.svg',
            name: 'Photoshop',
            rate: 4
          },
          { id: '13',
            icon: '/static/illustrator.svg',
            name: 'Illustrator',
            rate: 4
          }
        ]
      },
      interest: {
        title: '• Interest •',
        class: 'interest',
        item: [
          { id: '1',
            image: '/static/programming.svg',
            name: 'Programming'
          },
          { id: '2',
            image: '/static/design.svg',
            name: 'Design'
          },
          { id: '3',
            image: '/static/travelling.svg',
            name: 'Travelling'
          }
        ]
      },
      portfolio: {
        title: '• Portfolio •',
        class: 'portfolio',
        item: [
          { id: '1',
            logo: '/static/github.svg',
            username: 'rinaldydwii',
            link: 'https://github.com/rinaldydwii'
          },
          { id: '2',
            logo: '/static/behance.svg',
            username: 'rinaldydwii',
            link: 'https://behance.com/rinaldydwii'
          }
        ]
      },
      socialMedia: {
        title: '• Social Media •',
        class: 'social-media',
        item: [
          { id: '1',
            logo: '/static/facebook.svg',
            username: '/rinaldydwii',
            link: 'https://facebook.com/rinaldydwii'
          },
          { id: '2',
            logo: '/static/twitter.svg',
            username: '@rinaldydwii',
            link: 'https://twitter.com/rinaldydwii'
          },
          { id: '3',
            logo: '/static/instagram.svg',
            username: 'rinaldydwii',
            link: 'https://instagram.com/rinaldydwii'
          },
          { id: '4',
            logo: '/static/linkedin.svg',
            username: 'Rinaldy Dwi Istanto',
            link: 'https://linkedin.com/in/rinaldydwii'
          },
          { id: '5',
            logo: '/static/line.svg',
            username: 'aldyakakeju',
            link: 'http://line.me/ti/p/~aldyakakeju'
          },
          { id: '6',
            logo: '/static/whatsapp.svg',
            username: '+6281236001695',
            link: 'https://api.whatsapp.com/send?phone=6281236001695'
          }
        ]
      }
    }
  }
}
</script>
