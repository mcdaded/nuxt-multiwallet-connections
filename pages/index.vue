<template>
  <div class="w-full min-h-screen bg-black">
    <div class="mx-auto max-w-3xl pt-8">
      <div class="mx-auto max-w-3xl pt-8">
        <h1 class="text-4xl font-bold py-4 text-gray-50">Home Page</h1>
        <span
          class="text-blue-400 hover:underline hover:text-blue-600 pt-2 pb-8"
        >
          <Link href="/">Home</Link>
        </span>
        <div class="py-4 border rounded-lg my-4">
          <div class="p-6">
            <button
              @click="onClickConnectWallet1"
              class="inline-flex w-full items-center justify-center rounded-md border border-transparent bg-green-600 px-6 py-3 text-base font-medium text-white shadow-sm hover:bg-green-700 focus:outline-none focus:ring-2 focus:ring-green-500 focus:ring-offset-2"
            >
              Connect Wallet 1
            </button>
          </div>
          <div class="p-6">
            <form
              class="grid grid-cols-1 gap-y-6 sm:grid-cols-2 sm:gap-x-8 py-3 w-full items-center"
              @submit.prevent="onSendWalletTrans1"
            >
              <div class="mt-1 sm:col-span-2">
                <label class="block text-lg font-medium text-gray-50">
                  To Address
                </label>
                <div class="mt-1">
                  <input
                    v-model="wallet1trans.address"
                    type="text"
                    name="target"
                    id="target"
                    class="block w-full rounded-md border-gray-300 py-3 px-4 shadow-sm focus:border-indigo-500 focus:ring-indigo-500"
                  />
                </div>
              </div>
              <div class="mt-1 sm:col-span-2">
                <label class="block text-lg font-medium text-gray-50">
                  Amount
                </label>
                <div class="mt-1">
                  <input
                    v-model="wallet1trans.amount"
                    type="text"
                    name="amount"
                    id="amount"
                    class="block w-full rounded-md border-gray-300 py-3 px-4 shadow-sm focus:border-indigo-500 focus:ring-indigo-500"
                  />
                </div>
              </div>
              <div class="sm:col-span-2">
                <button
                  type="submit"
                  class="inline-flex w-full items-center justify-center rounded-md border border-transparent bg-indigo-600 px-6 py-3 text-base font-medium text-white shadow-sm hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-indigo-500 focus:ring-offset-2"
                >
                  Send Transaction
                </button>
              </div>
            </form>
          </div>
        </div>
        <div class="py-4 border rounded-lg mt-8">
          <div class="p-6">
            <button
              @click="onClickConnectWallet2"
              class="inline-flex w-full items-center justify-center rounded-md border border-transparent bg-green-600 px-6 py-3 text-base font-medium text-white shadow-sm hover:bg-green-700 focus:outline-none focus:ring-2 focus:ring-green-500 focus:ring-offset-2"
            >
              Connect Wallet 2
            </button>
          </div>
          <div class="p-6">
            <form
              class="grid grid-cols-1 gap-y-6 sm:grid-cols-2 sm:gap-x-8 py-3 w-full items-center"
              @submit.prevent="onSendWalletTrans2"
            >
              <div class="mt-1 sm:col-span-2">
                <label class="block text-lg font-medium text-gray-50">
                  To Address
                </label>
                <div class="mt-1">
                  <input
                    v-model="wallet2trans.address"
                    type="text"
                    name="target"
                    id="target"
                    class="block w-full rounded-md border-gray-300 py-3 px-4 shadow-sm focus:border-indigo-500 focus:ring-indigo-500"
                  />
                </div>
              </div>
              <div class="mt-1 sm:col-span-2">
                <label class="block text-lg font-medium text-gray-50">
                  Amount
                </label>
                <div class="mt-1">
                  <input
                    v-model="wallet2trans.amount"
                    type="text"
                    name="amount"
                    id="amount"
                    class="block w-full rounded-md border-gray-300 py-3 px-4 shadow-sm focus:border-indigo-500 focus:ring-indigo-500"
                  />
                </div>
              </div>
              <div class="sm:col-span-2">
                <button
                  type="submit"
                  class="inline-flex w-full items-center justify-center rounded-md border border-transparent bg-indigo-600 px-6 py-3 text-base font-medium text-white shadow-sm hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-indigo-500 focus:ring-offset-2"
                >
                  Send Transaction
                </button>
              </div>
            </form>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  data() {
    return {
      wallet1trans: {
        address: '',
        amount: '',
      },
      wallet2trans: {
        address: '',
        amount: '',
      },
    }
  },
  methods: {
    onClickConnectWallet1() {},
    onSendWalletTrans1() {},
    onClickConnectWallet2() {},
    onSendWalletTrans2() {},
  },
}
</script>
