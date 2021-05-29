<template>
  <!--Footer-->
  <footer class="bg-white">
    <div class="container mx-auto px-8">
      <div class="w-full flex flex-col md:flex-row py-6">
        <div class="flex-1 mb-6 text-black">
          <a
            class="
              text-pink-600
              no-underline
              hover:no-underline
              font-bold
              text-2xl
              lg:text-4xl
            "
            href="/"
          >
            <img
              class="h-10"
              src="/images/logo.png"
              alt="Thiết kế website ở Vĩnh Phúc"
            />
          </a>
          <ul class="list-reset my-6">
            <li class="mt-2 inline-block mr-2 md:block md:mr-0">
              <a
                href="https://facebook.com/lovanlong.ga"
                class="
                  no-underline
                  hover:underline
                  text-gray-800
                  hover:text-pink-500
                "
                >Facebook</a
              >
            </li>
            <li class="mt-2 inline-block mr-2 md:block md:mr-0">
              <a
                href="https://zalo.me/longitk"
                class="
                  no-underline
                  hover:underline
                  text-gray-800
                  hover:text-pink-500
                "
                >Zalo</a
              >
            </li>
            <li class="mt-2 inline-block mr-2 md:block md:mr-0">
              <a
                href="tel:0374638603"
                class="
                  no-underline
                  hover:underline
                  text-gray-800
                  hover:text-pink-500
                "
                >Gọi điện</a
              >
            </li>
          </ul>
        </div>
        <div class="flex-1 mb-6">
          <p class="uppercase text-gray-500 md:mb-6">Liên kết</p>
          <ul class="list-reset mb-6">
            <li class="mt-2 inline-block mr-2 md:block md:mr-0">
              <a
                href="#"
                class="
                  no-underline
                  hover:underline
                  text-gray-800
                  hover:text-pink-500
                "
                >FAQ</a
              >
            </li>
            <li class="mt-2 inline-block mr-2 md:block md:mr-0">
              <a
                href="#"
                class="
                  no-underline
                  hover:underline
                  text-gray-800
                  hover:text-pink-500
                "
                >Help</a
              >
            </li>
            <li class="mt-2 inline-block mr-2 md:block md:mr-0">
              <a
                href="#"
                class="
                  no-underline
                  hover:underline
                  text-gray-800
                  hover:text-pink-500
                "
                >Support</a
              >
            </li>
            <li class="mt-2 inline-block mr-2 md:block md:mr-0">
              <a
                href="#"
                class="
                  no-underline
                  hover:underline
                  text-gray-800
                  hover:text-pink-500
                "
                >Terms</a
              >
            </li>
            <li class="mt-2 inline-block mr-2 md:block md:mr-0">
              <a
                href="#"
                class="
                  no-underline
                  hover:underline
                  text-gray-800
                  hover:text-pink-500
                "
                >Privacy</a
              >
            </li>
          </ul>
        </div>
        <div class="flex-1 mb-6">
          <p class="uppercase text-gray-500 md:mb-6">Liên hệ chúng tôi</p>
          <p class="text-gray-500 md:mb-6">
            <em>Thiết kế trang web hiện đại</em>
          </p>
          <p class="text-gray-500 md:mb-6">
            217, Hai Bà Trưng <br />
            P. Hùng Vương<br />
            Phúc Yên, Vĩnh Phúc<br />
            Điện thoại: <a href="tel:0374638603">037 463 86 03</a> <br />
            Email: <a href="mailto:info@lovanlong.ga">info@lovanlong.ga</a>
          </p>
          <p class="text-gray-500 md:mb-6">
            Giá: Bắt đầu từ đ 5.000.000 <br />
            với các sản phẩm lớn hơn yêu cầu báo giá tùy chỉnh
          </p>
        </div>
        <div class="flex-1">
          <p class="uppercase text-gray-500 md:mb-6">Về chúng tôi</p>
          <p class="text-gray-500 md:mb-6">
            Chúng tôi là một công ty
            <strong>thiết kế web tại Vĩnh Phúc</strong> phục vụ khu vực Phúc Yên
            và các doanh nghiệp khác trên toàn Vĩnh Phúc. Chúng tôi tự hào về
            việc cung cấp mức độ dịch vụ được cá nhân hóa và nỗ lực tìm ra giải
            pháp cho nhu cầu của doanh nghiệp bạn. Mục tiêu của chúng tôi là
            giúp khách hàng của bạn tìm thấy bạn theo cách hiệu quả nhất có thể.
            Liên hệ với chúng tôi ngay hôm nay để lên lịch hẹn thảo luận về
            trang web mới của bạn.
          </p>
        </div>
      </div>
    </div>
    <a href="https://www.lovanlong.ga" class="text-gray-500"
      >Thiết kế trang web hiện đại - www.lovanlong.ga</a
    >
  </footer>
  <!-- jQuery if you need it
  <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
  -->
  <!-- <script>
    
  </script>
  <script>

  </script> -->
</template>
<script>
export default {
  mounted() {
    let scrollpos = window.scrollY
    const header = document.getElementById('header')
    const navcontent = document.getElementById('nav-content')
    const navaction = document.getElementById('navAction')
    const brandname = document.getElementById('brandname')
    const toToggle = document.querySelectorAll('.toggleColour')

    document.addEventListener('scroll', function () {
      /* Apply classes for slide in bar */
      scrollpos = window.scrollY

      if (scrollpos > 10) {
        header.classList.add('bg-white')
        navaction.classList.remove('bg-white')
        navaction.classList.add('gradient')
        navaction.classList.remove('text-gray-800')
        navaction.classList.add('text-white')
        // Use to switch toggleColour colours
        for (var i = 0; i < toToggle.length; i++) {
          toToggle[i].classList.add('text-gray-800')
          toToggle[i].classList.remove('text-white')
        }
        header.classList.add('shadow')
        navcontent.classList.remove('bg-gray-100')
        navcontent.classList.add('bg-white')
      } else {
        header.classList.remove('bg-white')
        navaction.classList.remove('gradient')
        navaction.classList.add('bg-white')
        navaction.classList.remove('text-white')
        navaction.classList.add('text-gray-800')
        // Use to switch toggleColour colours
        for (var i = 0; i < toToggle.length; i++) {
          toToggle[i].classList.add('text-white')
          toToggle[i].classList.remove('text-gray-800')
        }

        header.classList.remove('shadow')
        navcontent.classList.remove('bg-white')
        navcontent.classList.add('bg-gray-100')
      }
    })

    const navMenuDiv = document.getElementById('nav-content')
    const navMenu = document.getElementById('nav-toggle')

    document.onclick = check
    function check(e) {
      const target = (e && e.target) || (event && event.srcElement)

      // Nav Menu
      if (!checkParent(target, navMenuDiv)) {
        // click NOT on the menu
        if (checkParent(target, navMenu)) {
          // click on the link
          if (navMenuDiv.classList.contains('hidden')) {
            navMenuDiv.classList.remove('hidden')
          } else {
            navMenuDiv.classList.add('hidden')
          }
        } else {
          // click both outside link and outside menu, hide menu
          navMenuDiv.classList.add('hidden')
        }
      }
    }
    function checkParent(t, elm) {
      while (t.parentNode) {
        if (t == elm) {
          return true
        }
        t = t.parentNode
      }
      return false
    }
  },
}
</script>
