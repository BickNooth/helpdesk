<template>
  <div>
    <nav
      id="header"
      class="bg-white fixed w-full z-10 pin-t shadow"
    >
      <div class="w-full container mx-auto flex flex-wrap items-center mt-0 pt-3 pb-3 md:pb-0">
        <div class="w-1/2 pl-2 md:pl-0">
          <a
            class="text-black text-base xl:text-xl no-underline hover:no-underline font-bold"
            href="#"
          >
            <i class="fas fa-sun text-orange-dark pr-3" /> Admin Day Mode
          </a>
        </div>
        <div class="w-1/2 pr-0">
          <div class="flex relative inline-block float-right">
            <div class="relative text-sm">
              <button
                id="userButton"
                class="flex items-center focus:outline-none mr-3"
              >
                <img
                  class="w-8 h-8 rounded-full mr-4"
                  src="http://i.pravatar.cc/300"
                  alt="Avatar of User"
                > <span class="hidden md:inline-block">Hi, User </span>
                <svg
                  class="pl-2 h-2"
                  version="1.1"
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 129 129"
                  xmlns:xlink="http://www.w3.org/1999/xlink"
                  enable-background="new 0 0 129 129"
                ><g><path d="m121.3,34.6c-1.6-1.6-4.2-1.6-5.8,0l-51,51.1-51.1-51.1c-1.6-1.6-4.2-1.6-5.8,0-1.6,1.6-1.6,4.2 0,5.8l53.9,53.9c0.8,0.8 1.8,1.2 2.9,1.2 1,0 2.1-0.4 2.9-1.2l53.9-53.9c1.7-1.6 1.7-4.2 0.1-5.8z" /></g></svg>
              </button>
              <div
                id="userMenu"
                class="bg-white rounded shadow-md mt-2 absolute mt-12 pin-t pin-r min-w-full overflow-auto z-30 invisible"
              >
                <ul class="list-reset">
                  <li>
                    <a
                      href="#"
                      class="px-4 py-2 block text-black hover:bg-grey-light no-underline hover:no-underline"
                    >My account</a>
                  </li>
                  <li>
                    <a
                      href="#"
                      class="px-4 py-2 block text-black hover:bg-grey-light no-underline hover:no-underline"
                    >Notifications</a>
                  </li>
                  <li><hr class="border-t mx-2 border-grey-ligght"></li>
                  <li>
                    <a
                      href="#"
                      class="px-4 py-2 block text-black hover:bg-grey-light no-underline hover:no-underline"
                    >Logout</a>
                  </li>
                </ul>
              </div>
            </div>

            <div class="block lg:hidden pr-4">
              <button
                id="nav-toggle"
                class="flex items-center px-3 py-2 border rounded text-grey border-grey-dark hover:text-black hover:border-teal appearance-none focus:outline-none"
              >
                <svg
                  class="fill-current h-3 w-3"
                  viewBox="0 0 20 20"
                  xmlns="http://www.w3.org/2000/svg"
                ><title>Menu</title><path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z" /></svg>
              </button>
            </div>
          </div>
        </div>

        <div
          id="nav-content"
          class="w-full flex-grow lg:flex lg:items-center lg:w-auto hidden lg:block mt-2 lg:mt-0 bg-white z-20"
        >
          <ul class="list-reset lg:flex flex-1 items-center px-4 md:px-0">
            <li class="mr-6 my-2 md:my-0">
              <a
                href="#"
                class="block py-1 md:py-3 pl-1 align-middle text-orange-dark no-underline hover:text-black border-b-2 border-orange-dark hover:border-orange-dark"
              >
                <i class="fas fa-home fa-fw mr-3 text-orange-dark" /><span class="pb-1 md:pb-0 text-sm">Home</span>
              </a>
            </li>
            <li class="mr-6 my-2 md:my-0">
              <a
                href="#"
                class="block py-1 md:py-3 pl-1 align-middle text-grey no-underline hover:text-black border-b-2 border-white hover:border-pink"
              >
                <i class="fas fa-tasks fa-fw mr-3" /><span class="pb-1 md:pb-0 text-sm">Tasks</span>
              </a>
            </li>
            <li class="mr-6 my-2 md:my-0">
              <a
                href="#"
                class="block py-1 md:py-3 pl-1 align-middle text-grey no-underline hover:text-black border-b-2 border-white hover:border-purple"
              >
                <i class="fa fa-envelope fa-fw mr-3" /><span class="pb-1 md:pb-0 text-sm">Messages</span>
              </a>
            </li>
            <li class="mr-6 my-2 md:my-0">
              <a
                href="#"
                class="block py-1 md:py-3 pl-1 align-middle text-grey no-underline hover:text-black border-b-2 border-white hover:border-green"
              >
                <i class="fas fa-chart-area fa-fw mr-3" /><span class="pb-1 md:pb-0 text-sm">Analytics</span>
              </a>
            </li>
            <li class="mr-6 my-2 md:my-0">
              <a
                href="#"
                class="block py-1 md:py-3 pl-1 align-middle text-grey no-underline hover:text-black border-b-2 border-white hover:border-red"
              >
                <i class="fa fa-wallet fa-fw mr-3" /><span class="pb-1 md:pb-0 text-sm">Payments</span>
              </a>
            </li>
          </ul>

          <div class="relative pull-right pl-4 pr-4 md:pr-0">
            <input
              type="search"
              placeholder="Search"
              class="w-full bg-grey-lightest text-sm text-grey-darkest transition border focus:outline-none focus:border-grey-darker rounded py-1 px-2 pl-10 appearance-none leading-normal"
            >
            <div
              class="absolute search-icon"
              style="top: 0.375rem;left: 1.75rem;"
            >
              <svg
                class="fill-current pointer-events-none text-grey-darkest w-4 h-4"
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 20 20"
              >
                <path d="M12.9 14.32a8 8 0 1 1 1.41-1.41l5.35 5.33-1.42 1.42-5.33-5.34zM8 14A6 6 0 1 0 8 2a6 6 0 0 0 0 12z" />
              </svg>
            </div>
          </div>
        </div>
      </div>
    </nav>

    <!--Container-->
    <div class="container w-full mx-auto pt-20">
      <div class="w-full px-4 md:px-0 md:mt-8 mb-16 text-grey-darkest leading-normal">
        <!--Console Content-->

        <div class="flex flex-wrap">
          <div class="w-full md:w-1/2 xl:w-1/3 p-3">
            <!--Metric Card-->
            <div class="bg-white border rounded shadow p-2">
              <div class="flex flex-row items-center">
                <div class="flex-shrink pr-4">
                  <div class="rounded p-3 bg-green-dark">
                    <i class="fa fa-wallet fa-2x fa-fw fa-inverse" />
                  </div>
                </div>
                <div class="flex-1 text-right md:text-center">
                  <h5 class="uppercase text-grey">
                    Total Revenue
                  </h5>
                  <h3 class="text-3xl">
                    $3249 <span class="text-green"><i class="fas fa-caret-up" /></span>
                  </h3>
                </div>
              </div>
            </div>
            <!--/Metric Card-->
          </div>
          <div class="w-full md:w-1/2 xl:w-1/3 p-3">
            <!--Metric Card-->
            <div class="bg-white border rounded shadow p-2">
              <div class="flex flex-row items-center">
                <div class="flex-shrink pr-4">
                  <div class="rounded p-3 bg-orange-dark">
                    <i class="fas fa-users fa-2x fa-fw fa-inverse" />
                  </div>
                </div>
                <div class="flex-1 text-right md:text-center">
                  <h5 class="uppercase text-grey">
                    Total Users
                  </h5>
                  <h3 class="text-3xl">
                    249 <span class="text-orange"><i class="fas fa-exchange-alt" /></span>
                  </h3>
                </div>
              </div>
            </div>
            <!--/Metric Card-->
          </div>
          <div class="w-full md:w-1/2 xl:w-1/3 p-3">
            <!--Metric Card-->
            <div class="bg-white border rounded shadow p-2">
              <div class="flex flex-row items-center">
                <div class="flex-shrink pr-4">
                  <div class="rounded p-3 bg-yellow-dark">
                    <i class="fas fa-user-plus fa-2x fa-fw fa-inverse" />
                  </div>
                </div>
                <div class="flex-1 text-right md:text-center">
                  <h5 class="uppercase text-grey">
                    New Users
                  </h5>
                  <h3 class="text-3xl">
                    2 <span class="text-yellow-dark"><i class="fas fa-caret-up" /></span>
                  </h3>
                </div>
              </div>
            </div>
            <!--/Metric Card-->
          </div>
          <div class="w-full md:w-1/2 xl:w-1/3 p-3">
            <!--Metric Card-->
            <div class="bg-white border rounded shadow p-2">
              <div class="flex flex-row items-center">
                <div class="flex-shrink pr-4">
                  <div class="rounded p-3 bg-blue-dark">
                    <i class="fas fa-server fa-2x fa-fw fa-inverse" />
                  </div>
                </div>
                <div class="flex-1 text-right md:text-center">
                  <h5 class="uppercase text-grey">
                    Server Uptime
                  </h5>
                  <h3 class="text-3xl">
                    152 days
                  </h3>
                </div>
              </div>
            </div>
            <!--/Metric Card-->
          </div>
          <div class="w-full md:w-1/2 xl:w-1/3 p-3">
            <!--Metric Card-->
            <div class="bg-white border rounded shadow p-2">
              <div class="flex flex-row items-center">
                <div class="flex-shrink pr-4">
                  <div class="rounded p-3 bg-indigo-dark">
                    <i class="fas fa-tasks fa-2x fa-fw fa-inverse" />
                  </div>
                </div>
                <div class="flex-1 text-right md:text-center">
                  <h5 class="uppercase text-grey">
                    To Do List
                  </h5>
                  <h3 class="text-3xl">
                    7 tasks
                  </h3>
                </div>
              </div>
            </div>
            <!--/Metric Card-->
          </div>
          <div class="w-full md:w-1/2 xl:w-1/3 p-3">
            <!--Metric Card-->
            <div class="bg-white border rounded shadow p-2">
              <div class="flex flex-row items-center">
                <div class="flex-shrink pr-4">
                  <div class="rounded p-3 bg-red-dark">
                    <i class="fas fa-inbox fa-2x fa-fw fa-inverse" />
                  </div>
                </div>
                <div class="flex-1 text-right md:text-center">
                  <h5 class="uppercase text-grey">
                    Issues
                  </h5>
                  <h3 class="text-3xl">
                    3 <span class="text-red"><i class="fas fa-caret-up" /></span>
                  </h3>
                </div>
              </div>
            </div>
            <!--/Metric Card-->
          </div>
        </div>

        <!--Divider-->
        <hr class="border-b-2 border-grey-light my-8 mx-4">

        <div class="flex flex-row flex-wrap flex-grow mt-2">
          <div class="w-full md:w-1/2 p-3">
            <!--Graph Card-->
            <div class="bg-white border rounded shadow">
              <div class="border-b p-3">
                <h5 class="uppercase text-grey-dark">
                  Graph
                </h5>
              </div>
              <div class="p-5">
                <canvas
                  id="chartjs-7"
                  class="chartjs"
                  width="undefined"
                  height="undefined"
                />
              </div>
            </div>
            <!--/Graph Card-->
          </div>

          <div class="w-full md:w-1/2 p-3">
            <!--Graph Card-->
            <div class="bg-white border rounded shadow">
              <div class="border-b p-3">
                <h5 class="uppercase text-grey-dark">
                  Graph
                </h5>
              </div>
              <div class="p-5">
                <canvas
                  id="chartjs-0"
                  class="chartjs"
                  width="undefined"
                  height="undefined"
                />
              </div>
            </div>
            <!--/Graph Card-->
          </div>

          <div class="w-full md:w-1/2 xl:w-1/3 p-3">
            <!--Graph Card-->
            <div class="bg-white border rounded shadow">
              <div class="border-b p-3">
                <h5 class="uppercase text-grey-dark">
                  Graph
                </h5>
              </div>
              <div class="p-5">
                <canvas
                  id="chartjs-1"
                  class="chartjs"
                  width="undefined"
                  height="undefined"
                />
              </div>
            </div>
            <!--/Graph Card-->
          </div>

          <div class="w-full md:w-1/2 xl:w-1/3 p-3">
            <!--Graph Card-->
            <div class="bg-white border rounded shadow">
              <div class="border-b p-3">
                <h5 class="uppercase text-grey-dark">
                  Graph
                </h5>
              </div>
              <div class="p-5">
                <canvas
                  id="chartjs-4"
                  class="chartjs"
                  width="undefined"
                  height="undefined"
                />
              </div>
            </div>
            <!--/Graph Card-->
          </div>

          <div class="w-full md:w-1/2 xl:w-1/3 p-3">
            <!--Template Card-->
            <div class="bg-white border rounded shadow">
              <div class="border-b p-3">
                <h5 class="uppercase text-grey-dark">
                  Template
                </h5>
              </div>
              <div class="p-5" />
            </div>
            <!--/Template Card-->
          </div>

          <div class="w-full p-3">
            <!--Table Card-->
            <div class="bg-white border rounded shadow">
              <div class="border-b p-3">
                <h5 class="uppercase text-grey-dark">
                  Table
                </h5>
              </div>
              <div class="p-5">
                <table class="w-full p-5 text-grey-darker">
                  <thead>
                    <tr>
                      <th class="text-left text-blue-darkest">
                        Name
                      </th>
                      <th class="text-left text-blue-darkest">
                        Side
                      </th>
                      <th class="text-left text-blue-darkest">
                        Role
                      </th>
                    </tr>
                  </thead>

                  <tbody>
                    <tr>
                      <td>Obi Wan Kenobi</td>
                      <td>Light</td>
                      <td>Jedi</td>
                    </tr>
                    <tr>
                      <td>Greedo</td>
                      <td>South</td>
                      <td>Scumbag</td>
                    </tr>
                    <tr>
                      <td>Darth Vader</td>
                      <td>Dark</td>
                      <td>Sith</td>
                    </tr>
                  </tbody>
                </table>

                <p class="py-2">
                  <a href="#">See More issues...</a>
                </p>
              </div>
            </div>
            <!--/table Card-->
          </div>
        </div>

        <!--/ Console Content-->
      </div>
    </div>
    <!--/container-->

    <footer class="bg-white border-t border-grey-light shadow">
      <div class="container max-w-md mx-auto flex py-8">
        <div class="w-full mx-auto flex flex-wrap">
          <div class="flex w-full md:w-1/2 ">
            <div class="px-8">
              <h3 class="font-bold text-black">
                About
              </h3>
              <p class="py-4 text-grey-dark text-sm">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas vel mi ut felis tempus commodo nec id erat. Suspendisse consectetur dapibus velit ut lacinia.
              </p>
            </div>
          </div>

          <div class="flex w-full md:w-1/2">
            <div class="px-8">
              <h3 class="font-bold text-black">
                Social
              </h3>
              <ul class="list-reset items-center text-sm pt-3">
                <li>
                  <a
                    class="inline-block text-grey-dark no-underline hover:text-black hover:text-underline py-1"
                    href="#"
                  >Add social link</a>
                </li>
                <li>
                  <a
                    class="inline-block text-grey-dark no-underline hover:text-black hover:text-underline py-1"
                    href="#"
                  >Add social link</a>
                </li>
                <li>
                  <a
                    class="inline-block text-grey-dark no-underline hover:text-black hover:text-underline py-1"
                    href="#"
                  >Add social link</a>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>
