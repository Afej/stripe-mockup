<template>
  <div class="dashboard">
    <SideNav />
    <div class="main-content">
      <Header />
      <section class="payments">
        <div class="payments-header">
          <h1>Payments</h1>
          <div class="payments-buttons">
            <button>
              <svg
                width="16"
                height="17"
                viewBox="0 0 16 17"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M12.4982 2.5C12.9146 2.5 13.2529 2.83609 13.2529 3.25021C13.2528 3.4172 13.1968 3.57935 13.0939 3.71083L8.75617 9.25487L8.75167 12.7943C8.75175 12.893 8.73238 12.9907 8.69466 13.0818C8.65694 13.1729 8.60162 13.2558 8.53186 13.3255L7.37954 14.4778C7.3691 14.4883 7.35576 14.4955 7.34122 14.4985C7.32668 14.5015 7.31159 14.5 7.29786 14.4944C7.28413 14.4888 7.27237 14.4792 7.26408 14.4669C7.25578 14.4546 7.25132 14.4401 7.25126 14.4253V9.25487L2.90906 3.71083C2.84818 3.63314 2.80329 3.54414 2.777 3.449C2.7507 3.35385 2.74352 3.25444 2.75587 3.15651C2.76821 3.05857 2.79984 2.96405 2.84893 2.87841C2.89801 2.79277 2.96358 2.7177 3.04185 2.65754C3.17449 2.55532 3.33726 2.49992 3.50472 2.5H12.4982Z"
                  fill="#4F566B"
                />
              </svg>

              Filter
            </button>
            <button>
              <svg
                width="16"
                height="17"
                viewBox="0 0 16 17"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M14.0021 10.0575C14.0021 10.2801 13.9137 10.4935 13.7563 10.6509C13.5989 10.8083 13.3854 10.8967 13.1628 10.8967C12.9403 10.8967 12.7268 10.8083 12.5694 10.6509C12.412 10.4935 12.3236 10.2801 12.3236 10.0575V5.35766L3.42163 14.2563C3.34426 14.3336 3.25242 14.3949 3.15136 14.4367C3.05029 14.4785 2.94198 14.5 2.8326 14.5C2.72322 14.5 2.61492 14.4784 2.51389 14.4365C2.41285 14.3946 2.32105 14.3332 2.24374 14.2558C2.16643 14.1785 2.10511 14.0866 2.06329 13.9856C2.02147 13.8845 1.99996 13.7762 2 13.6668C2.00004 13.5574 2.02162 13.4491 2.06351 13.3481C2.10541 13.2471 2.16679 13.1553 2.24416 13.0779L11.1444 4.17935H6.44462C6.22193 4.17935 6.00835 4.09088 5.85088 3.93341C5.69341 3.77594 5.60495 3.56237 5.60495 3.33967C5.60495 3.11698 5.69341 2.9034 5.85088 2.74593C6.00835 2.58847 6.22193 2.5 6.44462 2.5H13.1754C13.2563 2.50104 13.3366 2.51376 13.4138 2.53777C13.5846 2.5899 13.7341 2.69569 13.84 2.83945C13.946 2.98322 14.0028 3.1573 14.0021 3.3359V10.0575Z"
                  fill="#4F566B"
                />
              </svg>
              Export
            </button>
            <button class="bg-blue">
              <svg
                width="16"
                height="17"
                viewBox="0 0 16 17"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M8.75 7.75H13.25C13.4489 7.75 13.6397 7.82902 13.7803 7.96967C13.921 8.11032 14 8.30109 14 8.5C14 8.69891 13.921 8.88968 13.7803 9.03033C13.6397 9.17098 13.4489 9.25 13.25 9.25H8.75V13.75C8.75 13.9489 8.67098 14.1397 8.53033 14.2803C8.38968 14.421 8.19891 14.5 8 14.5C7.80109 14.5 7.61032 14.421 7.46967 14.2803C7.32902 14.1397 7.25 13.9489 7.25 13.75V9.25H2.75C2.55109 9.25 2.36032 9.17098 2.21967 9.03033C2.07902 8.88968 2 8.69891 2 8.5C2 8.30109 2.07902 8.11032 2.21967 7.96967C2.36032 7.82902 2.55109 7.75 2.75 7.75H7.25V3.25C7.25 3.05109 7.32902 2.86032 7.46967 2.71967C7.61032 2.57902 7.80109 2.5 8 2.5C8.19891 2.5 8.38968 2.57902 8.53033 2.71967C8.67098 2.86032 8.75 3.05109 8.75 3.25V7.75Z"
                  fill="white"
                />
              </svg>
              Create payment
            </button>
          </div>
        </div>
        <nav class="payments-nav">
          <ul>
            <li>All</li>
            <li class="active">Succeeded</li>
            <li>Refunded</li>
            <li>Uncaptured</li>
          </ul>
        </nav>

        <div class="payments-table">
          <Payments :payments="payments" />
        </div>

        <footer class="payments-footer">
          <p class="footer-results">
            <span>{{ payments.length }}</span> Results
          </p>
          <div class="footer-buttons">
            <button class="prev">Previous</button>
            <button class="next">Next</button>
          </div>
        </footer>
      </section>
    </div>
  </div>
</template>

<script>
import Header from "@/components/Header";
import SideNav from "@/components/SideNav";
import Payments from "@/components/Payments";

export default {
  name: "Dashboard",
  components: {
    Header,
    SideNav,
    Payments,
  },
  data() {
    return {
      payments: [],
    };
  },
  created() {
    this.payments = [
      {
        id: 1,
        amount: "US$352.22",
        description: {
          text: "fe3d8216-58f9-4dc1-aaef-2f19463b5258",
          label: "Succeeded",
        },
        customer: "john.doe@gmail.com",
        date: "7 Jul, 14:04",
      },
      {
        id: 2,
        amount: "US$352.22",
        description: {
          text: "fe3d8216-58f9-4dc1-aaef-2f19463b5258",
          label: "Succeeded",
        },
        customer: "john.doe@gmail.com",
        date: "7 Jul, 14:04",
      },
      {
        id: 3,
        amount: "US$352.22",
        description: {
          text: "fe3d8216-58f9-4dc1-aaef-2f19463b5258",
          label: "Succeeded",
        },
        customer: "john.doe@gmail.com",
        date: "7 Jul, 14:04",
      },
      {
        id: 4,
        amount: "US$352.22",
        description: {
          text: "fe3d8216-58f9-4dc1-aaef-2f19463b5258",
          label: "Succeeded",
        },
        customer: "john.doe@gmail.com",
        date: "7 Jul, 14:04",
      },
      {
        id: 5,
        amount: "US$352.22",
        description: {
          text: "fe3d8216-58f9-4dc1-aaef-2f19463b5258",
          label: "Succeeded",
        },
        customer: "john.doe@gmail.com",
        date: "7 Jul, 14:04",
      },
      {
        id: 6,
        amount: "US$352.22",
        description: {
          text: "fe3d8216-58f9-4dc1-aaef-2f19463b5258",
          label: "Succeeded",
        },
        customer: "john.doe@gmail.com",
        date: "7 Jul, 14:04",
      },
      {
        id: 7,
        amount: "US$352.22",
        description: {
          text: "fe3d8216-58f9-4dc1-aaef-2f19463b5258",
          label: "Succeeded",
        },
        customer: "john.doe@gmail.com",
        date: "7 Jul, 14:04",
      },
      {
        id: 8,
        amount: "US$352.22",
        description: {
          text: "fe3d8216-58f9-4dc1-aaef-2f19463b5258",
          label: "Succeeded",
        },
        customer: "john.doe@gmail.com",
        date: "7 Jul, 14:04",
      },
      {
        id: 9,
        amount: "US$352.22",
        description: {
          text: "fe3d8216-58f9-4dc1-aaef-2f19463b5258",
          label: "Succeeded",
        },
        customer: "john.doe@gmail.com",
        date: "7 Jul, 14:04",
      },
      {
        id: 10,
        amount: "US$352.22",
        description: {
          text: "fe3d8216-58f9-4dc1-aaef-2f19463b5258",
          label: "Succeeded",
        },
        customer: "john.doe@gmail.com",
        date: "7 Jul, 14:04",
      },
      {
        id: 11,
        amount: "US$352.22",
        description: {
          text: "fe3d8216-58f9-4dc1-aaef-2f19463b5258",
          label: "Succeeded",
        },
        customer: "john.doe@gmail.com",
        date: "7 Jul, 14:04",
      },
      {
        id: 12,
        amount: "US$352.22",
        description: {
          text: "fe3d8216-58f9-4dc1-aaef-2f19463b5258",
          label: "Succeeded",
        },
        customer: "john.doe@gmail.com",
        date: "7 Jul, 14:04",
      },
      {
        id: 13,
        amount: "US$352.22",
        description: {
          text: "fe3d8216-58f9-4dc1-aaef-2f19463b5258",
          label: "Succeeded",
        },
        customer: "john.doe@gmail.com",
        date: "7 Jul, 14:04",
      },
      {
        id: 14,
        amount: "US$352.22",
        description: {
          text: "fe3d8216-58f9-4dc1-aaef-2f19463b5258",
          label: "Succeeded",
        },
        customer: "john.doe@gmail.com",
        date: "7 Jul, 14:04",
      },
      {
        id: 15,
        amount: "US$352.22",
        description: {
          text: "fe3d8216-58f9-4dc1-aaef-2f19463b5258",
          label: "Succeeded",
        },
        customer: "john.doe@gmail.com",
        date: "7 Jul, 14:04",
      },
      {
        id: 16,
        amount: "US$352.22",
        description: {
          text: "fe3d8216-58f9-4dc1-aaef-2f19463b5258",
          label: "Succeeded",
        },
        customer: "john.doe@gmail.com",
        date: "7 Jul, 14:04",
      },
    ];
  },
};
</script>

<style scoped>
.dashboard {
  display: flex;
  flex-direction: row;
  align-items: flex-start;
  padding: 0px;
  width: 100vw;
  height: 100vh;
  background: #ffffff;
}

.main-content {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  padding: 0px;
  /* min-width: 1156px; */
  width: 100%;
  margin-left: 250px;
  /* height: 873px; */
}

.main-content svg.checkbox {
  position: absolute;
  right: 0;
  top: 0;
}

.payments {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  padding: 0px 40px;
  /* min-width: 1156px; */
  margin: 32px 0px;
  width: 100%;
}

.payments-header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 100%;
}

.payments-header h1 {
  font-style: normal;
  font-weight: bold;
  font-size: 28px;
  line-height: 33px;
  color: #1a1f36;
}

.payments-buttons {
  display: flex;
}

.payments-buttons button {
  display: flex;
  align-items: center;
  background: #ffffff;
  box-shadow: 0px 2px 5px rgba(60, 66, 87, 0.08),
    0px 0px 0px 1px rgba(60, 66, 87, 0.16), 0px 1px 1px rgba(0, 0, 0, 0.12);
  border-radius: 4px;
  padding: 6px 8px;
  border: none;
  margin-right: 8px;
  color: #3c4257;
  cursor: pointer;
}

.payments-buttons button svg {
  margin-right: 8px;
}

button.bg-blue {
  background: #5469d4;
  color: #ffffff;
}

.payments-nav {
  margin: 20px 0px;
  border-bottom: 1px solid #e3e8ee;
  width: 100%;
}

.payments-nav ul {
  display: flex;
  align-items: flex-start;
}

.payments-nav ul li {
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  line-height: 17px;
  color: #697386;
  margin-right: 26px;
  cursor: pointer;
}

.payments-nav ul li.active {
  color: #5469d4;
  box-shadow: 0px 2px 0px #5469d4;
  padding: 0px 0px 9px;
}

.payments-table {
  width: 100%;
  overflow-x: auto;
}

.payments-footer {
  margin: 20px 0px;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.payments-footer p {
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 17px;
  color: #3c4257;
}

.payments-footer p span {
  font-weight: 600;
}

.footer-buttons button {
  padding: 6px 8px;
  color: #3c4257;
  background: #ffffff;
  opacity: 0.5;
  box-shadow: 0px 2px 5px rgba(60, 66, 87, 0.08),
    0px 0px 0px 1px rgba(60, 66, 87, 0.16), 0px 1px 1px rgba(0, 0, 0, 0.12);
  border-radius: 4px;
  border: none;
  margin: 0px 8px;
  cursor: pointer;
}

.footer-buttons button.next {
  color: #000;
  font-weight: bold;
}

/* media queries */
@media screen and (max-width: 768px) {
  .main-content {
    margin-left: 0px;
  }

  .payments {
    padding: 0px 20px;
  }
}

@media screen and (max-width: 540px) {
  .payments-header {
    display: flex;
    flex-direction: column;
    align-items: flex-start;  
  }

  .payments-buttons{
    margin-top: 12px;
  }
}
</style>