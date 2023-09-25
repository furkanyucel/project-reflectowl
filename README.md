# project-reflectowl
Simplays is a website that saves you time and money for expenses, invoices, refunds and much more



// Breakpoint Start
$xsMobile: 404px;
$mobile: 767px;
$tablet: 991px;
$smallDesktop: 1199px;
$largeDesktop: 1200px;


// Large Desktop Screen Start
@media (min-width: $largeDesktop) {
  .hero {
    @include flex-style(flex, column, center, auto);
  }
}
// Large Desktop Screen End


// Small Desktop Screen Start
@media (min-width: $smallDesktop) {
  .hero {
    // width: calc(100% - 280px);
    @include padding-style(auto, auto, 140, 140);
    @include flex-style(flex, row, center, auto);


    .hero-left {

      .main {
        
        h1 {
          width: 800px;
          @include custom-style(#000, 64px, 700, 70px, auto);
        }
      }
    }

    .hero-right {

      figure {
        img {
          width: 100%;
          max-width: 754px;
        }
      }
    }
  }
}
// Small Desktop Screen Start


// Tablet Screen Start
@media (min-width: $tablet) {}
// Tablet Screen End


// Mobile Screen Start
@media (min-width: $mobile) {}
// Mobile Screen End


//XS Mobile Screen Start
@media (max-width: $xsMobile) {
  header {
    height: 650px;
    @include padding-style(0, 0, 24, 24);
    @include flex-style(flex, column, center, center);

    figure {
      margin-bottom: 3rem;
    }

    nav {
      ul {
        @include flex-style(flex, column, center, center);
        row-gap: 2rem;
        text-align: center;

        li {
          margin-right: 0;
        }
      }
    }

    .login-signup {
      margin-top: 4rem;
      @include flex-style(flex, column, center, center);
      row-gap: 2rem;

      a {
        margin-left: 0 !important;
      }

      a:last-child {
        display: flex;
        margin-left: 0;
      }
    }
  }

  // Hero Start
.hero {
  @include margin-style(64, 64, 32, 32);
  @include flex-style(flex, column, center, center);

  .hero-left {
    

    .top {
      align-items: flex-end;
    }

    .main {
      margin-top: 2rem;
      width: 100%;
      max-width: 844px;
      @include flex-style(flex, column, flex-start, auto);

      h1 {
        font-size: 38px;
        line-height: 44px;
      }
      
      p {
        margin-top: 3rem;
        width: 100%;
        @include custom-style(#000, 14px, 400, 24px, -0.6px);
      }

      .subs {
        flex-direction: column;

        input {
          height: 64px;
          border: none;
        }
  
        button {
          margin-top: 16px;
          width: 100%;
          height: 64px;
          margin-left: 0;
        }
      }

      .statistics {
        margin-top: 100px;
        display: flex;
  
        article {
          margin-right: 3.75rem;
  
          h2 {
            @include custom-style(#000, 36px, 700, 0, auto);
          }
  
          p {
            margin-top: 3rem;
            @include custom-style(#B1B1B1, 14px, 400, 0, auto);
          }
        }
      }
    }

    // section {}




  }

  .hero-right {
    figure {
      margin-top: 58px;
      img {
        width: 100%;
        max-width: 754px;
      }
    }
  }
}
// Hero End

// Everything Start
.everything {
  @include margin-style(0, 0, auto, auto);
  @include padding-style(120, 0, auto, auto);
  @include flex-style(flex, column, auto, auto);
  background: #F2F4F5;

  h2 {
    margin-bottom: 120px;
    text-align: center;
    @include custom-style(#000, 30px, 700, 40px, -0.75px);
  }

  div {
    margin-top: 120px;

    article {
      @include padding-style(auto, auto, 32, 32);
      @include flex-style(flex, column, center, center);

      figure {
        display: flex;

        img {
          width: 100%;
          max-width: 576px;
        }
      }

      section {

        h2 {
          margin-top: -180px;
          width: 352px;
          text-align: left;
          @include custom-style(#000, 36px, 700, 40px, -0.75px);
        }

        p {
          width: 100%;
          margin-top: 1.125rem;
          @include custom-style(#000, 14px, 400, 22px, -0.35px);
        }

        a {
          margin-top: 1.75rem;
          text-align: right;
          @include custom-style(#fff, 14px, 700, 16px, auto);
          @include btn-style(#fff, #936EFE, 19px, 36px, 100px);

          &:hover {
            @include btn-style(#936EFE, #EDF860, 19px, 36px, 100px);
           outline: 3px dotted #936EFE;
          }
        }
      }
    }

    article {
      @include flex-style(flex, column, center, center);

      section {
        h2 {
          width: 100%;
        }

        p {
          width: 100%;
        }

        a {
          display: inline-flex;
          margin-top: 2.5rem;
          @include custom-style(#fff, 18px, 700, auto, auto);

          &:hover {
            background: #EDF860;
            color: #936EFE;
            outline: 3px dotted #936EFE;
          }
        }
      }

      figure {
        margin-top: -100px;
        order: -1;
      }
    }
  }

}
// Everything End


// Powerful Start
.powerful {
  @include padding-style(120, 120, 32, 32);

  h2 {
    text-align: center;
    @include custom-style(#000, 30px, 700, 40px, -0.75px);
  }

  .powerful-box {
    margin-top: 48px;
    @include flex-style(flex, column, center, auto);
    gap: 12px;

    section {
      @include padding-style(68, 20, 32, auto);
      width: 280px;
      height: 167px;

      h4 {
        @include custom-style(#000, 24px, 700, 0, -0.6px);
      }

      h5 {
        margin-top: 24px;
       @include custom-style(#000, 16px, 400, 14px, -0.4px);
      }

      p {
        margin-top: 16px;
        @include custom-style(#000, 12px, 400, 18px, 0);
      }
    }
  }
}
// Powerful End


// Time Start
.time {
  @include margin-style(0, 0, auto, auto);
  @include padding-style(120, 120, 32, 32);

  h2 {
    width: 100%;
    @include custom-style(#FFF, 28px, 700, 36px, -0.75px);

    &:last-of-type {
      width: 372px;
    }
  }

  p {
    width: 100%;
    margin-top: 18px;
    @include custom-style(#FFF, 14px, 400, 18px, 0.21px);
  }

  .time-photos {
    @include margin-style(64 , 120, auto, auto);
    column-gap: 10px;

    figure {

      &:hover {
        transform: translateY(-16px);
      }
    }

  }
}
// Time End


// Business Start
.business {
  @include padding-style(120, 100, 32, 32);
  @include flex-style(flex, column, center, center);

  .business-info {
    h2 {
      width: 288px;
      @include custom-style(#000, 30px, 700, 40px, -0.75px);
    }

    p {
      margin-top: 18px;
      width: 320px;
      @include custom-style(#000, 14px, 400, 22px, 0.21px);
    }

    a {
      margin-top: 24px;
      display: inline-flex;
      text-align: right;
      @include custom-style(#fff, 14px, 700, auto, auto);
      @include btn-style(#fff, #936EFE, 16px, 24px, 100px);

      &:hover {
        @include btn-style(#936EFE, #EDF860, 16px, 24px, 100px);
        outline: 3px dotted #936EFE;
      }
    }
  }

  .business-cards {
    margin-top: 50px;

    section {
      @include padding-style(36, auto, 22, 22);
      margin-bottom: 1.375rem;
      display: flex;
      width: 280px;
      height: 180px;
      border-radius: 30px;
      background: #936EFE;

      figure {
        margin-right: 10px;

        img {
          width: 100%;
        }

      }
      &:nth-of-type(1) {
        margin-left: 0;
      }

      &:nth-of-type(2) {
        margin-left: 0;
        background: #EDF860;
        p {
          color: #000;
        }
      }

      p {
        width: 374px;
        @include custom-style(#FFF, 14px, 400, 20px, -0.35px);
      }
    }
  }
}
// Business End


// Plans Start
.plan {
  @include padding-style(100, 80, 32, 32);
  @include flex-style(flex, column, auto, center);
  background: #F2F4F5;

  h2 {
    text-align: center;
    margin-bottom: 52px;
    width: 294px;
    @include custom-style(#000, 30px, 700, 40px, auto);
  }

  .plans {
    @include flex-style(flex, column, center, center);
    row-gap: 1.5rem;

    .plan-card {
      width: 280px;
      @include btn-style(auto, #FFF, 52px, 32px, 30px);

      h4 {
        @include custom-style(#000, 24px, 500, 30px, auto);
        text-align: left;
      }

      h6 {
        margin-top: 16px;
        width: 280px;
        @include custom-style(#000, 16px, 400, 20px, 0.3px);

        &:last-of-type {
          margin-top: 48px;
        }
      }

      h3 {
        @include custom-style(#000, 61px, 700, auto, -1.525px);
        margin-top: -0.5rem;
      }

      h5 {
        @include custom-style(#000, 16px, 400, auto, -0.35px);
        @include margin-style(8, 32, auto, auto);
      }

      .plan-card__info {

        p:before {
          margin-right: .75rem;
          content: "\f058";
          font-family: FontAwesome;
          color: #A3DC2F;
        }

        p {
          margin-top: 1rem;
          @include custom-style(#000, 16px, 400, 56px, 0.4px);
        }
      }

      .btn-plan {

        a {
          @include margin-style(52, 0, auto, auto);
          width: 180px;
          display: inline-flex;
          justify-content: center;
          border: 1px solid #000;
          background: none;
          @include custom-style(auto, 16px, 700, 20px, 0.4px);
          @include btn-style(#000, #fff, 14px, 50px, 100px);

          &:hover {
            border: transparent;
            color: #936EFE;
            background: #EDF860;
          }
        }
      }

      &:hover {
        transform: translateY(0px);
        background: #936EFE;

        h2, h3, h4, h5, h6, p {
          color: #FFF;
        }
          a {
            border: transparent;
            background: #fff;

            &:hover {
              border: #FFF;
            }
          }

      }
    }
  }
}
// Plans End


// Covered Start
.covered {
  @include padding-style(40, 80, 32, 32);
  @include flex-style(flex, column, center, flex-start);
  background: #F2F4F5;

  .covered-info {
    h2 {
      width: 236px;
      @include custom-style(#000, 30px, 700, 40px, auto);
    }

    p {
      width: 356px;
      margin-top: 1.125rem;
      margin-bottom: 3.5rem;
      @include custom-style(#000, 14px, 400, 22px, 0.21px);
    }

    a {
      margin-top: 0;
      margin-bottom: 50px;
      display: inline-flex;
      text-align: right;
      @include custom-style(#fff, 18px, 700, 0, auto);
      @include btn-style(auto, #936EFE, 28px, 36px, 100px);

      &:hover {
        background: #EDF860;
        color: #936EFE;
        outline: 3px dotted #936EFE;
      }
    }
  }
}
// Covered End


// Footer Start
.footer {
  @include flex-style(flex, column, auto, auto);
  @include padding-style(80, auto, 32, 32);
  background: #936EFE;

  .footer-top {
    display: grid;
    width: auto;
    grid-template-areas:
    "info"
    "nav"
    "address";

    .footer-basic {
      grid-area: info;

      h5 {
        margin-top: 14px;
        width: 300px;
        @include custom-style(#E4E4E4, 20, 400, 28px, 0.5px);
      }

      a {
        margin-top: 24px;
        display: inline-flex;
        @include custom-style(#000, 18px, 700, 0, auto);
        @include btn-style(auto, #fff, 28px, 36px, 100px);

        &:hover {
          color: #936EFE;
          background: #EDF860;
          outline: 3px dotted #EDF860;
        }
    }
    }

    .footer-nav {
      margin-top: 48px;
      grid-area: nav;
      display: grid;
      width: auto;
      grid-template-areas:
      "company"
      "help"
      "social"
      "address";
      row-gap: 48px;


      ul {

        h4 {
          @include custom-style(#fff, 24px, 700, auto, auto);
          padding-bottom: 16px;
        }

        li {
          padding-top: 16px;
          height: 32px;

          a {
            @include custom-style(#fff, 18px, 400, auto, 0.45px);

            &:hover {
              color: #EDF860;
            }
          }
        }
      }

      #address {
        grid-area: address;
        width: 100%;

        #map {
          margin-bottom: 60px;
          width: 100%;
          @include flex-style(inline-flex, column, center, flex-start);
          row-gap: 1rem;

          #pin {
            color: #A3DC2F;
            text-decoration: underline;
          }
        }

        #contact {
          margin-top: 20px;
          @include flex-style(inline-flex, column, center, flex-start);
          row-gap: 1rem;
        }
      }
    }
}

#footer-bottom {

    article {
      @include padding-style(32, 32, auto, auto);
      flex-direction: column;
      justify-content: flex-start;

      h6 {
        @include custom-style(#fff, 9px, 400, 30px, 0.5px);
      }
    }

}
}
// Footer End
}
//XS Mobile Screen End




// Breakpoint End










// $breakpoint-small: 576px;
// $breakpoint-medium: 768px;
// $breakpoint-large: 992px;


// @media (min-width: $breakpoint-medium) and (max-width: $breakpoint-large) {}