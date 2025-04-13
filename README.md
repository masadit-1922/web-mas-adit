import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Input } from "@/components/ui/input";

export default function Home() {
  return (
    <div className="min-h-screen bg-gray-100 flex flex-col items-center py-10">
      <header className="text-center mb-10">
        <h1 className="text-4xl font-bold text-blue-600">WIFI MURAH GRATIS BIAYA PASANG</h1>
        <p className="text-lg text-gray-700 mt-2">Solusi internet cepat dan hemat untuk Anda</p>
      </header>
  
      <section className="grid grid-cols-1 md:grid-cols-3 gap-6 max-w-6xl w-full px-4">
        <Card className="border border-gray-300">
          <CardContent className="text-center">
            <h2 className="text-2xl font-semibold text-blue-600">Paket Basic</h2>
            <p className="text-gray-700 mt-2">Kecepatan hingga 10-20 Mbps</p>
            <p className="text-gray-700 mt-1">Rp110.000/bulan</p>
            <Button className="mt-4 w-full">Pilih Paket</Button>
          </CardContent>
        </Card>

        <Card className="border border-gray-300">
          <CardContent className="text-center">
            <h2 className="text-2xl font-semibold text-blue-600">Paket Standard</h2>
            <p className="text-gray-700 mt-2">Kecepatan hingga 30 Mbps</p>
            <p className="text-gray-700 mt-1">Rp150.000/bulan</p>
            <Button className="mt-4 w-full">Pilih Paket</Button>
          </CardContent>
        </Card>

        <Card className="border border-gray-300">
          <CardContent className="text-center">
            <h2 className="text-2xl font-semibold text-blue-600">Paket Premium</h2>
            <p className="text-gray-700 mt-2">Kecepatan hingga 50 Mbps</p>
            <p className="text-gray-700 mt-1">Rp300.000/bulan</p>
            <Button className="mt-4 w-full">Pilih Paket</Button>
          </CardContent>
        </Card>
      </section>

      <section className="mt-10 w-full max-w-3xl px-4">
        <Card className="border border-gray-300">
          <CardContent>
            <h3 className="text-xl font-semibold text-blue-600 text-center">Hubungi Kami</h3>
            <p className="text-gray-700 text-center mt-2">
              Isi formulir di bawah ini untuk informasi lebih lanjut atau pemasangan.
            </p>
            <form className="mt-6 grid gap-4">
              <Input placeholder="Nama Anda" className="border border-gray-300" />
              <Input placeholder="Email Anda" className="border border-gray-300" />
              <Input placeholder="Nomor Telepon" className="border border-gray-300" />
              <textarea
                placeholder="Pesan Anda"
                className="border border-gray-300 rounded-md p-2 h-28"
              ></textarea>
              <Button type="submit" className="w-full">Kirim Pesan</Button>
            </form>
          </CardContent>
        </Card>
      </section>

      <footer className="mt-10 text-center text-gray-600">
        <p>&copy; 2025 Jasa Internet Murah. Semua Hak Dilindungi.</p>
      </footer>
    </div>
  );
}
