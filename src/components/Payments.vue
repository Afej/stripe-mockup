<template>
  <table>
    <thead>
      <tr>
        <th class="checkbox-icon">
          <CustomCheckbox />
        </th>
        <th class="amount">AMOUNT</th>
        <th class="description">DESCRIPTION</th>
        <th class="customer">CUSTOMER</th>
        <th class="date">DATE</th>
        <th class="more-icon"></th>
      </tr>
    </thead>
    <tbody :key="payment.id" v-for="payment in payments">
      <Payment :payment="payment" />
    </tbody>
  </table>
</template>

<script>
import Payment from "@/components/Payment";
import CustomCheckbox from "@/components/CustomCheckbox";

export default {
  name: "Payments",
  components: {
    Payment,
    CustomCheckbox,
  },
  props: {
    payments: Array,
  },
};
</script>

<style scoped>
table {
  border-collapse: collapse;
  width: 100%;
  margin-bottom: 26px;
}

th {
  border-bottom: 1px solid #e3e8ee;
  margin: 10px 0px;
  height: 26px;
  text-align: start;
  font-style: normal;
  font-weight: 500;
  font-size: 11px;
  line-height: 13px;
  text-transform: uppercase;
  color: #1a1f36;
}

th.description {
  padding-left: 40px;
}

@media screen and (max-width: 540px) {
  th.description {
    padding-left: 0px;
  }
}
</style>