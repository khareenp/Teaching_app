<template>
  <!-- //   This example requires updating your template:

    //   
    //   <html class="h-full bg-gray-100">
    //   <body class="h-full">
    //   ```
    // -->
  <div class="min-h-full bg-gray-200">
    <nav class="bg-indigo-700">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="flex items-center justify-between h-16">
          <div class="flex items-center">
            <div class="flex-shrink-0">
              <img
                class="h-8 w-8"
                src="https://tailwindui.com/img/logos/workflow-mark-indigo-300.svg"
                alt="Workflow"
              />
            </div>
            <div class="hidden md:block">
              <div class="ml-10 flex items-baseline space-x-4">
                <!-- Current: "bg-indigo-700 text-white", Default: "text-white hover:bg-indigo-500 hover:bg-opacity-75" -->

                <a
                  href="#"
                  class="bg-indigo-700 text-white px-3 py-2 rounded-md text-sm font-medium"
                  aria-current="page"
                >
                  Dashboard
                </a>
              </div>
            </div>
          </div>
          <div class="hidden md:block">
            <div class="ml-4 flex items-center md:ml-6">
              <button
                type="button"
                class="bg-indigo-500 p-1 rounded-full text-indigo-200 hover:text-white focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-offset-indigo-600 focus:ring-white"
              >
                <span class="sr-only">View notifications</span>

                <!-- Heroicon name: outline/bell -->

                <svg
                  class="h-6 w-6"
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                  aria-hidden="true"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M15 17h5l-1.405-1.405A2.032 2.032 0 0118 14.158V11a6.002 6.002 0 00-4-5.659V5a2 2 0 10-4 0v.341C7.67 6.165 6 8.388 6 11v3.159c0 .538-.214 1.055-.595 1.436L4 17h5m6 0v1a3 3 0 11-6 0v-1m6 0H9"
                  />
                </svg>
              </button>

              <!-- Profile dropdown -->

              <div class="ml-3 relative">
                <div>
                  <button
                    type="button"
                    class="max-w-xs bg-indigo-600 rounded-full flex items-center text-sm text-white focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-offset-indigo-600 focus:ring-white"
                    id="user-menu-button"
                    aria-expanded="false"
                    aria-haspopup="true"
                  >
                    <span class="sr-only">Open user menu</span>
                    <img
                      class="h-8 w-8 rounded-full"
                      src="https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80"
                      alt=""
                    />
                  </button>
                </div>

                <!--
                  Dropdown menu, show/hide based on menu state.
  
                  Entering: "transition ease-out duration-100"
                    From: "transform opacity-0 scale-95"
                    To: "transform opacity-100 scale-100"
                  Leaving: "transition ease-in duration-75"
                    From: "transform opacity-100 scale-100"
                    To: "transform opacity-0 scale-95"
                -->

                <div
                  class="origin-top-right absolute right-0 mt-2 w-48 rounded-md shadow-lg py-1 bg-white ring-1 ring-black ring-opacity-5 focus:outline-none"
                  role="menu"
                  aria-orientation="vertical"
                  aria-labelledby="user-menu-button"
                  tabindex="-1"
                >
                  <!-- Active: "bg-gray-100", Not Active: "" -->

                  <a
                    href="#"
                    class="block px-4 py-2 text-sm text-gray-700"
                    role="menuitem"
                    tabindex="-1"
                    id="user-menu-item-0"
                  >
                    Your Profile
                  </a>

                  <a
                    href="#"
                    class="block px-4 py-2 text-sm text-gray-700"
                    role="menuitem"
                    tabindex="-1"
                    id="user-menu-item-1"
                  >
                    Settings
                  </a>

                  <a
                    href="#"
                    class="block px-4 py-2 text-sm text-gray-700"
                    role="menuitem"
                    tabindex="-1"
                    id="user-menu-item-2"
                  >
                    Sign out
                  </a>
                </div>
              </div>
            </div>
          </div>
          <div class="-mr-2 flex md:hidden">
            <!-- Mobile menu button -->

            <button
              type="button"
              class="bg-indigo-00 inline-flex items-center justify-center p-2 rounded-md text-indigo-200 hover:text-white hover:bg-indigo-500 hover:bg-opacity-75 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-offset-indigo-600 focus:ring-white"
              aria-controls="mobile-menu"
              aria-expanded="false"
            >
              <span class="sr-only">Open main menu</span>

              <!--
                Heroicon name: outline/menu
  
                Menu open: "hidden", Menu closed: "block"
              -->

              <svg
                class="block h-6 w-6"
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
                aria-hidden="true"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M4 6h16M4 12h16M4 18h16"
                />
              </svg>

              <!--
                Heroicon name: outline/x
  
                Menu open: "block", Menu closed: "hidden"
              -->

              <svg
                class="hidden h-6 w-6"
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
                aria-hidden="true"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M6 18L18 6M6 6l12 12"
                />
              </svg>
            </button>
          </div>
        </div>
      </div>

      <!-- Mobile menu, show/hide based on menu state. -->

      <div class="md:hidden" id="mobile-menu">
        <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
          <!-- Current: "bg-indigo-700 text-white", Default: "text-white hover:bg-indigo-500 hover:bg-opacity-75" -->
        </div>
        <div class="pt-4 pb-3 border-t border-indigo-700">
          <div class="flex items-center px-5">
            <div class="flex-shrink-0">
              <img
                class="h-10 w-10 rounded-full"
                src="https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80"
                alt=""
              />
            </div>
            <div class="ml-3">
              <div class="text-base font-medium text-white">Tom Cook</div>
              <div class="text-sm font-medium text-indigo-300">
                tom@example.com
              </div>
            </div>
            <button
              type="button"
              class="ml-auto bg-indigo-700 flex-shrink-0 p-1 border-2 border-transparent rounded-full text-indigo-200 hover:text-white focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-offset-indigo-600 focus:ring-white"
            >
              <span class="sr-only">View notifications</span>

              <!-- Heroicon name: outline/bell -->

              <svg
                class="h-6 w-6"
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
                aria-hidden="true"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M15 17h5l-1.405-1.405A2.032 2.032 0 0118 14.158V11a6.002 6.002 0 00-4-5.659V5a2 2 0 10-4 0v.341C7.67 6.165 6 8.388 6 11v3.159c0 .538-.214 1.055-.595 1.436L4 17h5m6 0v1a3 3 0 11-6 0v-1m6 0H9"
                />
              </svg>
            </button>
          </div>
          <div class="mt-3 px-2 space-y-1">
            <a
              href="#"
              class="block px-3 py-2 rounded-md text-base font-medium text-white hover:bg-indigo-500 hover:bg-opacity-75"
            >
              Your Profile
            </a>

            <a
              href="#"
              class="block px-3 py-2 rounded-md text-base font-medium text-white hover:bg-indigo-500 hover:bg-opacity-75"
            >
              Settings
            </a>

            <a
              href="#"
              class="block px-3 py-2 rounded-md text-base font-medium text-white hover:bg-indigo-500 hover:bg-opacity-75"
            >
              Sign out
            </a>
          </div>
        </div>
      </div>
    </nav>

    <header class="bg-white shadow">
      <div class="max-w-7xl mx-auto py-6 px-4 sm:px-6 lg:px-8">
        <h1 class="text-3xl font-bold leading-tight text-gray-900"></h1>
      </div>
    </header>
    <main>
      <div class="max-w-7xl mx-auto py-6 sm:px-6 lg:px-8">
        <!-- Replace with your content -->

        <div class="px-4 py-4 sm:px-0">
          <!-- center console  -->
          <div class="rounded-lg shadow-lg bg-white">
            <!--  Teacher profile img, title, classes etc -->
            <div class="flex flex-col py-12">
              <div class="flex flex-row px-10 space-x-10">
                <img
                  class="h-20 w-20 rounded-full"
                  src="https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80"
                />
                <div class="flex flex-col space-y-1">
                  <p class="text-indigo-500 font-medium text-xl">Teacher</p>
                  <div class="flex flex-row">
                    <div class="flex flex-col mr-10">
                      <p>2</p>
                      <p class="text-gray-400">Classes</p>
                    </div>
                    <div class="flex flex-col">
                      <p>30</p>
                      <p class="text-gray-400">Students</p>
                    </div>
                  </div>
                </div>
              </div>
              <hr class="mt-6" />
              <!--  menu items: classes, students, grades  -->
              <div
                class="flex flex-row px-10 py-2 text-gray-700 font-light uppercase text-sm"
              >
                <a href="#" class="mr-10"> Classes </a>
                <a href="#" class="mr-10"> Students </a>
                <a href="#" class="mr-10"> Grades </a>
              </div>

              <!-- <hr class="w-32 h-1 rounded-full bg-sky-300" /> -->
              <!-- Highlighted item -->
              <div
                class="flex flex-row justify-between bg-indigo-700 items-center"
              >
                <p class="flex ml-10 h-9 text-white items-center">Science</p>
                <button
                  class="bg-white rounded-lg h-6 mr-4 px-3 text-indigo-700"
                >
                  Upload
                </button>
              </div>
              <!--  Sorting alphabetical  -->
              <!-- <div class="flex flex-row-reverse m-3 text-xs">
                <svg
                  class="flex items-center pl-1 text-indigo-500 w-3 h-3"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M19 9l-7 7-7-7"
                  ></path>
                </svg>
                <p class="ml-4 text-indigo-500">A - Z</p>
                <p class="text-gray-400">Sort by:</p>
              </div> -->
              <hr />
              <!--   worksheets  -->

              <div class="mt-8 ml-10 mr-10 flex flex-row h-screen space-x-10">
                <!-- worksheet 1 -->
                <ul
                  role="list"
                  class="grid grid-cols-1 gap-6 sm:grid-cols-2 lg:grid-cols-4"
                >
                  <li
                    class="h-72 col-span-1 bg-white rounded-lg shadow-lg border-2"
                  >
                    <img
                      class="w-full h-32 bg-gray-300 rounded-t-lg flex-shrink-0"
                      src="https://i.pinimg.com/originals/b3/07/bf/b307bf46ee3b565331a3ffc5df587d3c.gif"
                      alt=""
                    />
                    <div class="w-64 flex items-center px-4 py-1">
                      <div class="flex-1 truncate">
                        <p class="mt-1 text-gray-500 text-sm truncate">
                          Worksheet description
                        </p>
                      </div>
                    </div>
                    <!-- edit/delete links -->
                    <div>
                      <div class="mt-14 flex divide-x divide-gray-300">
                        <div class="w-0 flex-1 flex">
                          <a
                            href="#"
                            class="relative -mr-px w-0 flex-1 inline-flex items-center justify-center py-4 text-sm text-gray-500 font-medium border border-transparent rounded-bl-lg hover:text-gray-500"
                          >
                            <!-- Heroicon name: edit/pencil -->
                            <svg
                              xmlns="http://www.w3.org/2000/svg"
                              class="h-5 w-5"
                              fill="none"
                              viewBox="0 0 24 24"
                              stroke="currentColor"
                              stroke-width="2"
                            >
                              <path
                                stroke-linecap="round"
                                stroke-linejoin="round"
                                d="M15.232 5.232l3.536 3.536m-2.036-5.036a2.5 2.5 0 113.536 3.536L6.5 21.036H3v-3.572L16.732 3.732z"
                              />
                            </svg>
                            <span class="ml-3">Edit</span>
                          </a>
                        </div>
                        <div class="-ml-px w-0 flex-1 flex">
                          <a
                            href="#"
                            class="relative w-0 flex-1 inline-flex items-center justify-center py-4 text-sm text-gray-700 font-medium border border-transparent rounded-br-lg hover:text-gray-500"
                          >
                            <!-- Heroicon name: Delete -->
                            <svg
                              xmlns="http://www.w3.org/2000/svg"
                              class="h-5 w-5 text-gray-400"
                              viewBox="0 0 20 20"
                              fill="currentColor"
                            >
                              <path
                                fill-rule="evenodd"
                                d="M9 2a1 1 0 00-.894.553L7.382 4H4a1 1 0 000 2v10a2 2 0 002 2h8a2 2 0 002-2V6a1 1 0 100-2h-3.382l-.724-1.447A1 1 0 0011 2H9zM7 8a1 1 0 012 0v6a1 1 0 11-2 0V8zm5-1a1 1 0 00-1 1v6a1 1 0 102 0V8a1 1 0 00-1-1z"
                                clip-rule="evenodd"
                              />
                            </svg>
                            <span class="ml-3">Delete</span>
                          </a>
                        </div>
                      </div>
                    </div>
                  </li>
                  <!-- Worksheet 2 -->
                  <li
                    class="h-72 col-span-1 bg-white rounded-lg shadow-lg border-2"
                  >
                    <img
                      class="w-full h-32 bg-gray-300 rounded-t-lg flex-shrink-0"
                      src="https://i.pinimg.com/originals/b3/07/bf/b307bf46ee3b565331a3ffc5df587d3c.gif"
                      alt=""
                    />
                    <div class="w-64 flex items-center px-4 py-1">
                      <div class="flex-1 truncate">
                        <p class="mt-1 text-gray-500 text-sm truncate">
                          Worksheet description
                        </p>
                      </div>
                    </div>
                    <!-- edit/delete links -->
                    <div>
                      <div class="mt-14 flex divide-x divide-gray-300">
                        <div class="w-0 flex-1 flex">
                          <a
                            href="#"
                            class="relative -mr-px w-0 flex-1 inline-flex items-center justify-center py-4 text-sm text-gray-500 font-medium border border-transparent rounded-bl-lg hover:text-gray-500"
                          >
                            <!-- Heroicon name: edit/pencil -->
                            <svg
                              xmlns="http://www.w3.org/2000/svg"
                              class="h-5 w-5"
                              fill="none"
                              viewBox="0 0 24 24"
                              stroke="currentColor"
                              stroke-width="2"
                            >
                              <path
                                stroke-linecap="round"
                                stroke-linejoin="round"
                                d="M15.232 5.232l3.536 3.536m-2.036-5.036a2.5 2.5 0 113.536 3.536L6.5 21.036H3v-3.572L16.732 3.732z"
                              />
                            </svg>
                            <span class="ml-3">Edit</span>
                          </a>
                        </div>
                        <div class="-ml-px w-0 flex-1 flex">
                          <a
                            href="#"
                            class="relative w-0 flex-1 inline-flex items-center justify-center py-4 text-sm text-gray-700 font-medium border border-transparent rounded-br-lg hover:text-gray-500"
                          >
                            <!-- Heroicon name: Delete -->
                            <svg
                              xmlns="http://www.w3.org/2000/svg"
                              class="h-5 w-5 text-gray-400"
                              viewBox="0 0 20 20"
                              fill="currentColor"
                            >
                              <path
                                fill-rule="evenodd"
                                d="M9 2a1 1 0 00-.894.553L7.382 4H4a1 1 0 000 2v10a2 2 0 002 2h8a2 2 0 002-2V6a1 1 0 100-2h-3.382l-.724-1.447A1 1 0 0011 2H9zM7 8a1 1 0 012 0v6a1 1 0 11-2 0V8zm5-1a1 1 0 00-1 1v6a1 1 0 102 0V8a1 1 0 00-1-1z"
                                clip-rule="evenodd"
                              />
                            </svg>
                            <span class="ml-3">Delete</span>
                          </a>
                        </div>
                      </div>
                    </div>
                  </li>

                  <!-- More worksheets... -->
                </ul>
              </div>
            </div>
          </div>
        </div>
        <!-- /End replace -->
      </div>
    </main>
  </div>
</template>
<style scoped></style>
